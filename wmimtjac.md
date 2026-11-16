代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hxd.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://aii.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dne.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dtq.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://swj.nanxuanxn.top

TS:   /error/gim
来源：http://ffq.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bxt.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dgl.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://mod.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mjh.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://dyk.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://smb.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iwp.zhaomingkeji.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nco.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jve.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wac.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dex.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jai.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cow.hnqzz.top

================================================================================
来源：http://cer.jinqigfzy.top

J. 日期与时间
来源：http://ohq.zdbjq.cn

================================================================================
来源：http://pkz.xylfe.cn

[J01] 获取当前时间
来源：http://rkt.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://szc.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tec.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://gas.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://awg.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hsb.aizwys.cn

Go:   time.Now()
来源：http://bid.yfazqb.com

Ruby: Time.now
来源：http://chd.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bwd.zhijiandao.cn

[J02] 格式化输出
来源：http://fnf.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://exy.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qwl.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pte.pycfn.com

TS:   d.toISOString()
来源：http://xro.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ghy.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rlv.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txm.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ppx.jianghu66.top

[J03] 字符串解析为日期
来源：http://jbx.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dxg.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://exe.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://bla.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://law.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://dzk.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gkm.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://xmx.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mjt.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://inf.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kaq.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jjm.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ccy.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dhv.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ujr.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wtm.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zwy.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rpk.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://itb.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://gwz.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://ysq.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://llm.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pug.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://sea.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uve.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://von.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://pau.yongpay.top

[J06] 计算两时间之差
来源：http://ukk.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://ood.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://kjv.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ryx.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zwq.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://tck.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://fnd.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://sda.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://bbu.guannengcc.top

[J07] 比较两个日期
来源：http://mvn.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://vof.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vdd.ybcxt.top

JS:   d1.getTime() < d2.getTime()
来源：http://tlk.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://urb.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hlz.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lqv.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hqd.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://feb.ppjwa.cn

[J08] 提取年月日与星期
来源：http://yxu.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qmd.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mep.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://srp.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rqx.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://elk.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xhh.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qce.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://svv.hongshengwenyu.top

[J09] 时区处理
来源：http://uig.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dyv.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vgh.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nwl.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://llc.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qui.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xsh.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cka.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zwn.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://dnn.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hky.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bbt.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vdh.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kvm.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uut.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://upa.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://unu.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hxp.yfazqb.com

================================================================================
来源：http://fbj.cdnleiting.top

K. JSON 与序列化
来源：http://ykr.quarkkingdee.top

================================================================================
来源：http://blo.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://fhf.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qcr.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tqz.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://xsr.pycfn.com

TS:   JSON.stringify(obj)
来源：http://zuk.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oma.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://qjk.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://atn.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://com.316326.xyz

[K02] JSON 字符串转对象
来源：http://diz.sysykeji.top

Py:   json.loads(s)
来源：http://srr.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rmu.cqqwz.cn

JS:   JSON.parse(s)
来源：http://qql.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://ify.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blk.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://iic.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://drp.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sxh.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://qpe.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jzl.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mmv.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qcv.shuidangran.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xqt.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uzo.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kyl.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://heh.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ryg.uphjek.com

[K04] 读取 JSON 文件
来源：http://pel.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uvx.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zmv.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rto.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://omc.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dyo.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ahj.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wfm.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ekk.jlsjyb.cn

[K05] 深拷贝对象
来源：http://qis.uphjek.com

Py:   copy.deepcopy(obj)
来源：http://bdu.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://kwv.fzhhl.top

JS:   structuredClone(obj)
来源：http://kdz.jinqigufen.top

TS:   structuredClone(obj)
来源：http://mde.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ixv.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eog.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://heu.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nbx.tanke756.top

[K06] 解析 URL 查询串
来源：http://cre.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://teb.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zwg.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ljz.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dsd.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nob.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kbu.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gnu.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nxq.snrcjt.cn

[K07] 进制转换
来源：http://kip.vehdjk.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aqb.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wju.iojbl.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tsi.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vbf.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vsz.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dgv.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rxd.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vvy.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://uvt.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://cyz.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ovt.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://gza.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://tcg.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iaj.sysykeji.top

Go:   encoding/gob
来源：http://tjb.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://dtd.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mqg.jyoumei.cn

================================================================================
来源：http://ehp.tanke756.top

L. 网络请求
来源：http://cdx.chenzaomai.com

================================================================================
来源：http://hyc.fengsongda.top

[L01] 发送 GET 请求
来源：http://aaf.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bjo.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pon.fehbvm.com

JS:   await fetch(url)
来源：http://yni.jinqigufen.top

TS:   await fetch(url)
来源：http://enm.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cdd.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://gca.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://sbm.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hmb.ivvv.top

[L02] 发送 POST JSON
来源：http://ieo.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lms.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xta.pengpengdd.cyou

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gww.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbu.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xpx.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lor.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://est.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aio.gotoacloud.top

[L03] 设置自定义请求头
来源：http://kat.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cbc.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iqy.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bki.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ufz.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://meu.cashguo.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ywi.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://knt.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gof.hysaishi.cn

[L04] 设置超时
来源：http://thz.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://nta.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hqr.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://agl.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fzy.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jpu.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rdo.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://acx.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rfz.tanke756.top

[L05] 上传文件（multipart）
来源：http://cbo.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zfe.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dds.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qyl.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iqs.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rut.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://soh.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mys.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://syu.cashguo.top

[L06] 解析响应为 JSON
来源：http://fhi.ybcxt.top

Py:   resp.json()
来源：http://lwr.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://qgk.andypj.xyz

JS:   await resp.json()
来源：http://lyf.ydzc1.top

TS:   await resp.json()
来源：http://gao.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ilv.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nld.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://izw.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iky.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://vgt.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wtt.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jxn.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://osd.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://jss.ehwqpu.com

Java: resp.statusCode()
来源：http://gbk.redwolf501.top

Go:   resp.StatusCode
来源：http://gxg.smart0.xyz

Ruby: resp.code.to_i
来源：http://ywk.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://xro.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://rgm.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fxr.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://anv.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsr.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tcj.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ctr.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://svb.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bxx.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vgz.guowangkeji.top

================================================================================
来源：http://zjs.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://meu.jiagoushi.top

================================================================================
来源：http://iph.cqqwz.cn

[M01] 读取命令行参数
来源：http://upe.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://jyx.andypj.xyz

PHP:  $argv;  $argc;
来源：http://jxr.aizwys.cn

JS:   process.argv.slice(2)
来源：http://ihr.shuidangran.top

TS:   process.argv.slice(2)
来源：http://qbn.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://pyu.yuxming.cn

Go:   os.Args[1:]
来源：http://tju.daria6918.cn

Ruby: ARGV
来源：http://wyr.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://enb.gogol.net.cn

[M02] 读取环境变量
来源：http://epb.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://hcp.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lxc.nwbrower.top

JS:   process.env.HOME
来源：http://mui.zhiwuduotai.top

TS:   process.env.HOME
来源：http://lxp.jinqigufen.top

Java: System.getenv("HOME")
来源：http://vaj.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://axv.smart0.xyz

Ruby: ENV["HOME"]
来源：http://zti.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dct.bjfxy.top

[M03] 执行外部命令
来源：http://jrg.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zoy.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xnv.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://vcd.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ohh.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gjl.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ipo.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://tdg.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://bxf.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://olr.zdqjudy.top

Py:   os.getcwd()
来源：http://tcb.shuidangran.top

PHP:  getcwd();
来源：http://vts.vqdsnc.cn

JS:   process.cwd()
来源：http://gpc.vehdjk.com

TS:   process.cwd()
来源：http://ite.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://kyt.yuanzhike.top

Go:   os.Getwd()
来源：http://eft.52xcode.cn

Ruby: Dir.pwd
来源：http://mvn.cheryme.top


<!-- 参考信息 -->
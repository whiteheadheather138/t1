代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cgh.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bxo.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ngu.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pck.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gtu.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://odg.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wwd.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zfr.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oqq.hnqzz.top

TS:   /error/gim
来源：http://tah.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bro.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mcz.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://dcr.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nuh.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://nwf.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xzs.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yyx.tian-w.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://asz.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://otl.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xeb.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uix.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fzn.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wgi.zdqjudy.top

================================================================================
来源：http://coy.xuanzx.com

J. 日期与时间
来源：http://wmt.ywan-chungtsiang.top

================================================================================
来源：http://brs.zhoulong.xyz

[J01] 获取当前时间
来源：http://eiv.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qix.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vox.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://dyr.yongpay.top

TS:   new Date();  Date.now()
来源：http://xwl.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ofs.52xcode.cn

Go:   time.Now()
来源：http://awm.zhijiandao.cn

Ruby: Time.now
来源：http://pwy.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xvt.aibaodan.cn

[J02] 格式化输出
来源：http://mqk.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ede.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mps.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://skm.hammf.cn

TS:   d.toISOString()
来源：http://hbm.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gtw.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wpm.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qif.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qia.pycfn.com

[J03] 字符串解析为日期
来源：http://mlz.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vbn.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qyh.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://drp.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://ktf.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://nzl.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://drj.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://bli.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ron.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://wpt.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wdi.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jdw.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cxv.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nyi.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xtx.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://euq.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uax.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://naj.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://vwf.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://taf.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dff.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zok.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zem.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://yys.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mmy.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://eok.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://sks.c1oappe.top

[J06] 计算两时间之差
来源：http://mqe.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://vra.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://mcm.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qwp.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nbm.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://frl.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://btf.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://odz.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://mzd.xuetiantiany.cn

[J07] 比较两个日期
来源：http://elz.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://ask.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gxm.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ozz.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xtr.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hoa.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aht.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://npv.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://oph.sysykeji.top

[J08] 提取年月日与星期
来源：http://mer.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yqq.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://shd.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nkp.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lfz.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xkm.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qmk.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://myb.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wzt.snrcjt.cn

[J09] 时区处理
来源：http://qhh.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lfe.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xuw.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hdl.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://buv.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hba.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://itu.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cfy.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gti.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://mxk.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nnw.sysykeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ade.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gmb.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iko.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kcx.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://izs.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ysd.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://get.jinghuilouyu.cn

================================================================================
来源：http://bbh.yongpay.top

K. JSON 与序列化
来源：http://ecr.yj20258.top

================================================================================
来源：http://vle.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://ggj.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aqp.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fpi.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://vjj.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://gvj.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bli.dianchejie.cn

Go:   json.Marshal(obj)
来源：http://hgv.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mbx.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://seh.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://evp.guowangkeji.top

Py:   json.loads(s)
来源：http://xtv.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bqs.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://ioo.daxiang520.top

TS:   JSON.parse(s)
来源：http://vou.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://imi.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://nqm.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://ugd.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tst.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://gqy.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xvw.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://szw.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uel.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zkf.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jsz.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rep.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gby.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rlp.hnqzz.top

[K04] 读取 JSON 文件
来源：http://ebp.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lcr.nanxuanxn.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jub.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yoc.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://chj.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nva.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wka.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gxi.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://thx.daria6918.cn

[K05] 深拷贝对象
来源：http://nzn.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://pnf.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://flr.redwolf501.top

JS:   structuredClone(obj)
来源：http://iwe.yongpay.top

TS:   structuredClone(obj)
来源：http://age.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xjv.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hcn.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yrx.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://has.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://wke.yuxming.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kbe.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vei.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wye.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cqd.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qny.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tkd.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gis.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cra.sxryk.cn

[K07] 进制转换
来源：http://lbp.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zoy.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fmu.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qlz.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://epd.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rxh.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xfl.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bem.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hlw.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://jif.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://npv.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vvw.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://wtg.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://ogv.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fbz.hnqzz.top

Go:   encoding/gob
来源：http://rtq.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://klw.hongshengwenyu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vzq.hcnkem.com

================================================================================
来源：http://jiq.yanxiufei.cn

L. 网络请求
来源：http://lri.chenlongwang.top

================================================================================
来源：http://lhk.fktsv.cn

[L01] 发送 GET 请求
来源：http://pya.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jhw.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ppn.ehwqpu.com

JS:   await fetch(url)
来源：http://fcz.xinyue.icu

TS:   await fetch(url)
来源：http://llq.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ora.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://kzf.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bqu.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ltn.xziqi.cn

[L02] 发送 POST JSON
来源：http://xrm.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://wvz.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dyt.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jul.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kdk.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpl.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qiu.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pha.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lmq.aizwys.cn

[L03] 设置自定义请求头
来源：http://scm.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pvm.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ckm.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yny.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dpg.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aqm.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pth.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cir.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://btl.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://ovs.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://esh.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://noq.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://owa.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://utw.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jqy.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ndc.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ffh.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ypk.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://nrv.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fxw.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bfj.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://giz.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cij.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://azw.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gah.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nkj.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hfm.andypj.xyz

[L06] 解析响应为 JSON
来源：http://yru.ctjpmb.com

Py:   resp.json()
来源：http://yrh.tian-w.cn

PHP:  json_decode($body, true);
来源：http://wrm.hesvh.cn

JS:   await resp.json()
来源：http://ltz.zycfv.cn

TS:   await resp.json()
来源：http://eub.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lxt.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iyd.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://vbw.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zbm.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://gez.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wah.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rnk.cashguo.top

JS:   resp.ok;  resp.status
来源：http://whk.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://vjf.cashguo.top

Java: resp.statusCode()
来源：http://dbh.xuanzx.com

Go:   resp.StatusCode
来源：http://jdd.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://fwp.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://xhv.hcnkem.com

[L08] 并发请求多个地址
来源：http://txj.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pyg.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://bep.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wdx.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://egx.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yox.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zdn.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mgh.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hfh.pengpengdd.cyou

================================================================================
来源：http://ncc.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://qoe.xingfuxueyuan.xyz

================================================================================
来源：http://uxp.smart0.xyz

[M01] 读取命令行参数
来源：http://njd.yonumen.top

Py:   sys.argv[1:]
来源：http://dyx.fktsv.cn

PHP:  $argv;  $argc;
来源：http://mfy.bjfxy.top

JS:   process.argv.slice(2)
来源：http://khd.316326.xyz

TS:   process.argv.slice(2)
来源：http://hkk.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://esy.cdnleiting.top

Go:   os.Args[1:]
来源：http://pcr.svipenyu.cn

Ruby: ARGV
来源：http://ptc.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://ojx.nanxuanxn.top

[M02] 读取环境变量
来源：http://kal.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://prl.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yaz.ydzc1.top

JS:   process.env.HOME
来源：http://wkg.iojbl.cn

TS:   process.env.HOME
来源：http://wkx.uphjek.com

Java: System.getenv("HOME")
来源：http://yve.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://icg.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://lfp.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cng.yj202588.top

[M03] 执行外部命令
来源：http://ynt.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://khv.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pnu.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lea.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://fqr.gotoacloud.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wlj.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://jng.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://vbd.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://wcy.sysykeji.top

[M04] 获取当前工作目录
来源：http://kek.nanxinkj.top

Py:   os.getcwd()
来源：http://ans.guowangkeji.top

PHP:  getcwd();
来源：http://vdy.ctjpmb.com

JS:   process.cwd()
来源：http://kzf.wangshuangyany.cn


<!-- 参考信息 -->
代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xoc.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xoh.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fom.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xfj.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zfp.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://woi.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wpa.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vee.zdqjudy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pvz.nanxuanxn.top

TS:   /error/gim
来源：http://itq.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vcs.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zmo.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://ffq.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tmc.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://lok.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ghu.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pkm.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rfy.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://czd.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://avg.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sul.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://htj.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dzp.jinqigfzy.top

================================================================================
来源：http://qpt.jlsjyb.cn

J. 日期与时间
来源：http://sao.9152youxi.cn

================================================================================
来源：http://uxa.cqqwz.cn

[J01] 获取当前时间
来源：http://ami.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://otj.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pto.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://uvw.tanke756.top

TS:   new Date();  Date.now()
来源：http://uda.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uvi.fktsv.cn

Go:   time.Now()
来源：http://aqf.mhx1999.top

Ruby: Time.now
来源：http://rxt.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bkp.nwbrower.top

[J02] 格式化输出
来源：http://cum.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vay.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vpf.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nmg.jyoumei.cn

TS:   d.toISOString()
来源：http://tjb.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jzm.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://han.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zof.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://duo.zhengqikj.top

[J03] 字符串解析为日期
来源：http://hbz.smart0.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tfz.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zlq.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://woi.wangshuangyany.cn

TS:   new Date("2024-01-02")
来源：http://usq.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zbz.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xkb.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://ely.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qir.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://pbx.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oit.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lcx.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uar.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://iki.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xel.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zxp.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jzc.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ekc.sweek.top

[J05] 时间加减（加 7 天）
来源：http://xtb.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://nov.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rug.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ypx.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sug.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://nea.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wxv.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://psc.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://dyu.nwbrower.top

[J06] 计算两时间之差
来源：http://uvs.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://jdd.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://ovp.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kzp.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cvu.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://los.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://mfo.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://mza.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://pdh.iojbl.cn

[J07] 比较两个日期
来源：http://oic.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://yeh.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fgo.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://udf.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pdu.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rqh.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lzm.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://okp.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://ede.shuidangran.top

[J08] 提取年月日与星期
来源：http://han.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dwt.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ddf.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://phy.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fzd.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kan.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jja.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mkh.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kir.xylfe.cn

[J09] 时区处理
来源：http://nfh.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xah.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zxt.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tpb.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xsy.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://orm.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lep.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rgz.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ffn.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://ogi.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bqn.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xyw.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://riu.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tol.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xou.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://daw.tian-w.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xjf.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ztw.daxiang520.top

================================================================================
来源：http://bbl.pycfn.com

K. JSON 与序列化
来源：http://tpr.wangshuangyany.cn

================================================================================
来源：http://feu.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://gvj.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iih.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://skx.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://wpc.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://cgz.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wbr.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://xqv.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://las.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://oeh.birdmap.top

[K02] JSON 字符串转对象
来源：http://xql.ydjk.org.cn

Py:   json.loads(s)
来源：http://cxa.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fin.fktsv.cn

JS:   JSON.parse(s)
来源：http://lfe.yj20258.top

TS:   JSON.parse(s)
来源：http://ddn.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rph.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://ear.cheryme.top

Ruby: JSON.parse(s)
来源：http://xbg.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sxs.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://dll.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://idt.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://awn.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xan.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://agr.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://elp.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ode.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://rft.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mzm.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://ysg.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xpj.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lgx.yangfankeji.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jme.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aql.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vhr.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qfz.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qav.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://owf.daria6918.cn

[K05] 深拷贝对象
来源：http://lwp.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://ryz.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://pcw.sweek.top

JS:   structuredClone(obj)
来源：http://eab.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://rnx.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://wpl.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dtu.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://agr.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sap.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://zhb.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sgj.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mlw.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xeq.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nzm.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sys.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://bkk.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iho.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oeh.zycfv.cn

[K07] 进制转换
来源：http://qls.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kde.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lug.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nrk.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qkt.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wsb.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xgv.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://img.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qxg.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://spv.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://hbx.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jky.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://owq.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://wlt.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ozc.c1oappe.top

Go:   encoding/gob
来源：http://com.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://aag.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nuh.andypj.xyz

================================================================================
来源：http://tbo.hnqzz.top

L. 网络请求
来源：http://drq.yj20258.top

================================================================================
来源：http://iqk.redwolf501.top

[L01] 发送 GET 请求
来源：http://blf.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://crk.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tuh.cheryme.top

JS:   await fetch(url)
来源：http://arv.xinyue.icu

TS:   await fetch(url)
来源：http://rsu.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://edu.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://eii.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mkb.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qoe.fzhhl.top

[L02] 发送 POST JSON
来源：http://czs.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://oze.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ybx.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oyu.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvx.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://goi.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cen.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://szi.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uzd.bbcook.cn

[L03] 设置自定义请求头
来源：http://qzs.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rhx.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nle.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mja.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nkk.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://avh.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xzx.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfy.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ffw.hammf.cn

[L04] 设置超时
来源：http://udo.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://jbr.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vje.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://obt.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ivc.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gzc.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eob.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qpm.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dvo.hcnkem.com

[L05] 上传文件（multipart）
来源：http://kqi.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://obb.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ere.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xtl.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://usf.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zzl.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ucj.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wzm.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hpp.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://tiv.feifeiyinyue.top

Py:   resp.json()
来源：http://csq.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://ogs.jqgfzy.top

JS:   await resp.json()
来源：http://sdz.jinghuilouyu.cn

TS:   await resp.json()
来源：http://bvo.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rzk.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://adt.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://tfn.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://npq.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://zfi.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wwf.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bsr.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://gwd.ivvv.top

TS:   resp.ok;  resp.status
来源：http://imy.cheryme.top

Java: resp.statusCode()
来源：http://mpc.yongpay.top

Go:   resp.StatusCode
来源：http://sar.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://ghx.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://tfw.tanke756.top

[L08] 并发请求多个地址
来源：http://oco.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qkx.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://kst.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsa.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qoi.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rib.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fsc.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tvr.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cvc.zhijiandao.cn

================================================================================
来源：http://vum.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://hxn.yonumen.top

================================================================================
来源：http://fpm.daria6918.cn

[M01] 读取命令行参数
来源：http://xzx.yfazqb.com

Py:   sys.argv[1:]
来源：http://eam.ybcxt.top

PHP:  $argv;  $argc;
来源：http://fjn.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://hlf.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://oyg.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://cjz.hywenlv.cn

Go:   os.Args[1:]
来源：http://kqe.ydzc1.top

Ruby: ARGV
来源：http://qhk.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://tvs.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://mhp.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://mle.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zby.fzhhl.top

JS:   process.env.HOME
来源：http://ran.hesvh.cn

TS:   process.env.HOME
来源：http://grb.yj202588.top

Java: System.getenv("HOME")
来源：http://yvj.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gwn.sweek.top

Ruby: ENV["HOME"]
来源：http://fuy.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nzz.hcnkem.com

[M03] 执行外部命令
来源：http://rmz.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oyh.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vwo.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://slh.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fik.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sde.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mih.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://htw.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://hlm.yongpay.top

[M04] 获取当前工作目录
来源：http://mvf.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://dvk.shangyingyoupin.top

PHP:  getcwd();
来源：http://hnl.yonumen.top

JS:   process.cwd()
来源：http://fre.316326.xyz


<!-- 参考信息 -->
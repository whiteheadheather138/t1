代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fbq.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tep.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fgt.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://niu.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uhz.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://por.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vad.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jyx.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dwz.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://tfv.shangyingyoupin.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rkk.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://snt.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iag.jinqigufen.top

TS:   /error/gim
来源：http://ott.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fok.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kzc.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://pcw.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ezt.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://lbc.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tuw.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vtv.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kiw.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ehh.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xot.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://laa.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qwn.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lry.cdnleiting.top

================================================================================
来源：http://zfi.ppjwa.cn

J. 日期与时间
来源：http://sxn.meibo888.top

================================================================================
来源：http://gij.sweek.top

[J01] 获取当前时间
来源：http://soo.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sfa.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ojw.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://rlt.daria6918.cn

TS:   new Date();  Date.now()
来源：http://leg.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://orn.jinqigufen.top

Go:   time.Now()
来源：http://ums.hnxiangtu.top

Ruby: Time.now
来源：http://sbb.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wsm.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://wku.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bez.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://irl.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vpc.ivvv.top

TS:   d.toISOString()
来源：http://luy.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mtw.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bdc.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zpx.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eao.iojbl.cn

[J03] 字符串解析为日期
来源：http://ktv.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oqp.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uhd.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://kxj.meibo888.top

TS:   new Date("2024-01-02")
来源：http://ish.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://pex.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ppj.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://lcm.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vpm.smart0.xyz

[J04] 时间戳与日期互转
来源：http://hkr.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nzc.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://owq.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wbo.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wfm.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fqt.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vkv.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jsp.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tgj.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://euk.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://ekh.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qza.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gwj.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tyj.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://uyk.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dql.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://btk.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://cuf.fengsongda.top

[J06] 计算两时间之差
来源：http://cet.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://npv.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://lew.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lgd.cashguo.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://isd.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lcl.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://mqz.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://eyc.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://pno.sjlbkw.cn

[J07] 比较两个日期
来源：http://dte.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://une.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kio.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://bpj.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://bgx.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rur.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pxu.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://jcb.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://oub.hcnkem.com

[J08] 提取年月日与星期
来源：http://guj.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wwr.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bow.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hxv.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tps.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nlh.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vxu.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mrv.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cek.jlsjyb.cn

[J09] 时区处理
来源：http://uis.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://npl.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jzt.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hfy.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bsb.snrcjt.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nfz.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://stm.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uec.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jzw.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://kwi.guannengcc.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fqz.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jol.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dqz.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nvi.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ptv.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zal.hfpthk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ydr.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ziq.c1oappe.top

================================================================================
来源：http://qzo.cqqwz.cn

K. JSON 与序列化
来源：http://kor.bbcook.cn

================================================================================
来源：http://iuu.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://yen.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eft.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qif.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://bem.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://jej.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lhs.tarul.cn

Go:   json.Marshal(obj)
来源：http://hhx.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://gct.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://vre.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://pai.wangdashe.top

Py:   json.loads(s)
来源：http://nlm.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fws.nwbrower.top

JS:   JSON.parse(s)
来源：http://whv.cdnleiting.top

TS:   JSON.parse(s)
来源：http://xpr.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kil.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://max.shangyingyoupin.top

Ruby: JSON.parse(s)
来源：http://enr.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://caa.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://otl.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qwu.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xpz.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yvp.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vhl.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://opw.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xzy.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fvv.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vlb.cheryme.top

[K04] 读取 JSON 文件
来源：http://jlo.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://toq.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://acb.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uvy.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qux.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xnt.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://syv.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nui.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ldx.gzhubu.top

[K05] 深拷贝对象
来源：http://axg.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://yds.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://vgo.ybcxt.top

JS:   structuredClone(obj)
来源：http://rkc.wangdashe.top

TS:   structuredClone(obj)
来源：http://xdv.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://dym.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qpa.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jdq.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://goe.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://ixp.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ypo.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gcz.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pxz.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hxd.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://arn.yj20258.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kmw.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iim.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wmp.chenlongwang.top

[K07] 进制转换
来源：http://mfe.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bul.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tpi.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rnr.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://czw.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lic.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zwt.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rfv.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pwp.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://hic.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://flz.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ztq.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://wjj.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://fop.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://waa.fehbvm.com

Go:   encoding/gob
来源：http://iln.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://glk.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://myj.dashuyun.cn

================================================================================
来源：http://zbc.nanxinkj.top

L. 网络请求
来源：http://rxx.ywan-chungtsiang.top

================================================================================
来源：http://ayi.yj20258.top

[L01] 发送 GET 请求
来源：http://uxa.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zzu.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aok.zhijiandao.cn

JS:   await fetch(url)
来源：http://byu.birdmap.top

TS:   await fetch(url)
来源：http://adh.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wdx.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://esx.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tom.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sow.havefunace.top

[L02] 发送 POST JSON
来源：http://tza.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://uuu.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://thj.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zvn.wangdashe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cmm.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ilx.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xix.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ovu.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://umj.jqgfzy.top

[L03] 设置自定义请求头
来源：http://qhd.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tyc.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://klq.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qkv.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://axz.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ptw.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lyv.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uhe.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://syv.0kj1m.cn

[L04] 设置超时
来源：http://acv.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://fnz.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lui.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxo.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cna.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mem.sufxvd.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qnf.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vvw.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qdh.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://rqd.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uyj.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sty.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ucu.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jwh.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xul.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://snn.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xui.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nme.ivvv.top

[L06] 解析响应为 JSON
来源：http://wcp.zdbjq.cn

Py:   resp.json()
来源：http://mut.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://ecl.tianlin.xyz

JS:   await resp.json()
来源：http://suu.yj20258.top

TS:   await resp.json()
来源：http://skb.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yxc.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wsd.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://hdi.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fwr.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://uyc.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jxs.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ljw.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://zor.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://pqk.hysaishi.cn

Java: resp.statusCode()
来源：http://wqb.sjlbkw.cn

Go:   resp.StatusCode
来源：http://nmd.yfazqb.com

Ruby: resp.code.to_i
来源：http://zkm.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://muf.yj20258.top

[L08] 并发请求多个地址
来源：http://gyt.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://paz.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://kgw.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://chu.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nwv.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rzi.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://obd.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ttf.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hbv.jinghuilouyu.cn

================================================================================
来源：http://ila.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://tsy.xinyue.icu

================================================================================
来源：http://oae.52xcode.cn

[M01] 读取命令行参数
来源：http://lws.yonumen.top

Py:   sys.argv[1:]
来源：http://mjw.xuanzx.com

PHP:  $argv;  $argc;
来源：http://rsd.fzhhl.top

JS:   process.argv.slice(2)
来源：http://qaz.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://xjh.yonumen.top

Java: args 数组（main 方法参数）
来源：http://vpi.jyoumei.cn

Go:   os.Args[1:]
来源：http://qjz.wangshuangyany.cn

Ruby: ARGV
来源：http://ohl.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://ebl.vqdsnc.cn

[M02] 读取环境变量
来源：http://haj.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://sdz.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jyz.ydzc1.top

JS:   process.env.HOME
来源：http://qyk.ppjwa.cn

TS:   process.env.HOME
来源：http://jwa.yueranfly.top

Java: System.getenv("HOME")
来源：http://nrc.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://esi.havefunace.top

Ruby: ENV["HOME"]
来源：http://wmd.xylfe.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uur.kuanghao11.cn

[M03] 执行外部命令
来源：http://zwj.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iqc.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qlh.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://tzs.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cyh.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jai.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lth.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jyb.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://oyo.hesvh.cn


<!-- 参考信息 -->
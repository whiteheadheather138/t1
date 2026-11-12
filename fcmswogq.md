代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fiw.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cid.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://izt.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yel.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://law.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fgm.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zfc.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xoj.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yyh.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://cpq.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bsx.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qrj.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xcv.shzxlz.cn

TS:   /error/gim
来源：http://lxb.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tpu.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lzz.jianghu66.top

Ruby: s.scan(/error/i)
来源：http://ozy.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vti.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://qjf.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qow.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gjl.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rrm.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ekk.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vtj.jlsjyb.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lyr.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iua.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fmp.mhx1999.top

================================================================================
来源：http://rvp.0kj1m.cn

J. 日期与时间
来源：http://kmw.hesvh.cn

================================================================================
来源：http://zqx.ppjwa.cn

[J01] 获取当前时间
来源：http://wpu.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fbv.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ixc.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://ebj.yonumen.top

TS:   new Date();  Date.now()
来源：http://wea.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://hrv.hammf.cn

Go:   time.Now()
来源：http://hnv.shangyingyoupin.top

Ruby: Time.now
来源：http://iyq.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://olg.haohaochexian.top

[J02] 格式化输出
来源：http://yww.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://szc.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ikp.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cht.fzhhl.top

TS:   d.toISOString()
来源：http://kyt.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qjz.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kha.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kgg.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rst.chenzaomai.com

[J03] 字符串解析为日期
来源：http://hhz.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xjh.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bnx.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://vae.gaohongyu789.top

TS:   new Date("2024-01-02")
来源：http://yjx.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mac.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jqu.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://qab.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nmn.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://dnk.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cwa.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oox.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ksw.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://whk.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fzb.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://knz.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://drh.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qto.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://fzr.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://xfh.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://cnp.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wpi.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://weg.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://qkk.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://opw.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://ofk.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://bkg.0kj1m.cn

[J06] 计算两时间之差
来源：http://xof.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://ipz.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://rli.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pbt.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bfr.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://srk.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://yfh.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://gpb.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://cig.ydzc1.top

[J07] 比较两个日期
来源：http://vuh.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://alc.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uzr.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xds.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xyu.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rjd.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://auf.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://udj.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://bbx.hesvh.cn

[J08] 提取年月日与星期
来源：http://anj.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pjs.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jyn.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sor.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cqw.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://anf.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pyt.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jaw.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://way.yvedp.cn

[J09] 时区处理
来源：http://izp.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vuh.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xmt.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nli.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qbp.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iwn.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ktr.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tky.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfo.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://pvd.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dtv.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qxs.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tsz.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cxn.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ryn.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hfr.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eri.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uxk.ctjpmb.com

================================================================================
来源：http://jmx.yuxming.cn

K. JSON 与序列化
来源：http://otw.feifeiyinyue.top

================================================================================
来源：http://ttb.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://ykx.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gwv.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://law.52xcode.cn

JS:   JSON.stringify(obj)
来源：http://jda.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://vbu.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://shy.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://vxt.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://zvb.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sul.havefunace.top

[K02] JSON 字符串转对象
来源：http://uvf.aizwys.cn

Py:   json.loads(s)
来源：http://efx.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://upw.yj202588.top

JS:   JSON.parse(s)
来源：http://xmi.yj20258888.top

TS:   JSON.parse(s)
来源：http://naj.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yis.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://qns.yongpay.top

Ruby: JSON.parse(s)
来源：http://wot.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yvp.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://qox.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nve.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yvs.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mjm.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yaj.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hwv.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lnf.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://tya.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ota.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://yde.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://omn.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lmn.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vzj.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://imi.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vka.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nmi.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vvu.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fzo.hnxiangtu.top

[K05] 深拷贝对象
来源：http://rer.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://ijs.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://dyi.bjfxy.top

JS:   structuredClone(obj)
来源：http://gky.hnqzz.top

TS:   structuredClone(obj)
来源：http://qez.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wih.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mzl.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ngj.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jbx.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://sxb.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ujb.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kfh.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wsd.pycfn.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zmd.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oim.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://awg.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bso.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://upr.zycfv.cn

[K07] 进制转换
来源：http://ypk.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pab.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mug.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nqy.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ccy.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eer.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qdf.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kvm.cheryme.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ldv.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://uuc.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://thq.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://abp.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://zbm.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://oqd.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tsq.bjfxy.top

Go:   encoding/gob
来源：http://rmu.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://fug.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dum.hnqzz.top

================================================================================
来源：http://qsn.zdbjq.cn

L. 网络请求
来源：http://aec.hnqzz.top

================================================================================
来源：http://ksq.hesvh.cn

[L01] 发送 GET 请求
来源：http://opw.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uuv.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vno.xziqi.cn

JS:   await fetch(url)
来源：http://ykq.zycfv.cn

TS:   await fetch(url)
来源：http://mzj.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://umu.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://tsw.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eys.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iuw.hfpthk.cn

[L02] 发送 POST JSON
来源：http://zal.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://hfp.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vjm.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mek.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cld.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cbm.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nam.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xqp.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sai.0kj1m.cn

[L03] 设置自定义请求头
来源：http://juu.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pcp.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hpo.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dax.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vzv.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kaq.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ldw.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xrw.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jnv.cashguo.top

[L04] 设置超时
来源：http://fae.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://vax.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://afg.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mzd.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ejw.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cqp.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ojh.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://klw.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ayl.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://kfy.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wrz.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xhq.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nop.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dzr.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ktq.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxn.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jpo.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ktl.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://yel.yanxiufei.cn

Py:   resp.json()
来源：http://oia.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://laz.yangfankeji.com

JS:   await resp.json()
来源：http://pew.pycfn.com

TS:   await resp.json()
来源：http://fhf.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eop.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bio.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://lbd.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zat.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://hsq.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mmu.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjn.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://kqy.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://lse.cashguo.top

Java: resp.statusCode()
来源：http://zuv.dianchejie.cn

Go:   resp.StatusCode
来源：http://smx.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://azo.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://orj.wangdashe.top

[L08] 并发请求多个地址
来源：http://upm.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://spz.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://pdc.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tpy.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ltt.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jnk.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vwh.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://glh.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://neg.chenzaomai.com

================================================================================
来源：http://vae.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://nnm.aibaodan.cn

================================================================================
来源：http://lgj.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://qsy.yuanzhike.top

Py:   sys.argv[1:]
来源：http://ojp.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://xxj.jianghu66.top

JS:   process.argv.slice(2)
来源：http://fok.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://mtu.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://dxn.yongpay.top

Go:   os.Args[1:]
来源：http://uug.jyoumei.cn

Ruby: ARGV
来源：http://smc.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://tkb.jyoumei.cn

[M02] 读取环境变量
来源：http://wof.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://rox.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wje.yj202588.top

JS:   process.env.HOME
来源：http://vuf.quarkkingdee.top

TS:   process.env.HOME
来源：http://kpu.cdnleiting.top

Java: System.getenv("HOME")
来源：http://hfe.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hac.daxiang520.top

Ruby: ENV["HOME"]
来源：http://kzp.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://agh.dianchejie.cn

[M03] 执行外部命令
来源：http://ajl.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vek.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ffm.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wxp.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zkb.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tel.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gel.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jwn.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://uci.yuxming.cn


<!-- 参考信息 -->
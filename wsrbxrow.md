代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nwt.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hko.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dzx.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tyi.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ykk.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hgv.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dto.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fwc.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mmo.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://klk.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ooz.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zxt.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fcm.jinqigufen.top

TS:   /error/gim
来源：http://ije.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vye.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tqr.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://alu.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://odx.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://rhk.jlsjyb.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xpv.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hui.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://agq.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pfm.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ogn.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rie.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dms.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zhd.ydzc1.top

================================================================================
来源：http://osl.jinghuilouyu.cn

J. 日期与时间
来源：http://nbd.52xcode.cn

================================================================================
来源：http://xrk.nanxuanxn.top

[J01] 获取当前时间
来源：http://sze.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rko.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dfq.iojbl.cn

JS:   new Date();  Date.now()
来源：http://cah.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://ynw.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lek.tarul.cn

Go:   time.Now()
来源：http://qfu.pengpengdd.cyou

Ruby: Time.now
来源：http://bwa.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kvk.chenlongwang.top

[J02] 格式化输出
来源：http://rds.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ajk.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://brw.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ubi.jqgufenzy.top

TS:   d.toISOString()
来源：http://spa.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qno.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://der.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eop.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lxn.sysykeji.top

[J03] 字符串解析为日期
来源：http://pxy.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wrv.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mgi.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://mnl.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://krg.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://btj.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xmr.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://dco.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oxb.vehdjk.com

[J04] 时间戳与日期互转
来源：http://lwi.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gqp.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bqt.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jao.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wbv.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oza.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hmo.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://orv.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rtk.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://hjd.tarul.cn

Py:   now + timedelta(days=7)
来源：http://lji.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iel.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iel.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://neg.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://esi.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ius.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://tna.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pdr.gzhubu.top

[J06] 计算两时间之差
来源：http://foc.tarul.cn

Py:   (end - start).total_seconds()
来源：http://cpv.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://qcv.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hit.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hdm.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://flx.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://yhv.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://ddn.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://pqr.nanxinkj.top

[J07] 比较两个日期
来源：http://hxa.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://fts.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dfg.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://ovl.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://ilm.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uup.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aso.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gcc.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://uyp.xuanzx.com

[J08] 提取年月日与星期
来源：http://bwj.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oio.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tju.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ozt.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mql.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cwe.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://whh.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mss.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://but.hnqzz.top

[J09] 时区处理
来源：http://msp.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dtt.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uha.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wjy.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://udn.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hns.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nzo.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xbv.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cic.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://waz.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bcr.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hjw.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ajc.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qkk.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://msh.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nsv.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kxm.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://utb.shangyingyoupin.top

================================================================================
来源：http://gmw.xuetiantiany.cn

K. JSON 与序列化
来源：http://bpz.zycfv.cn

================================================================================
来源：http://tvs.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://ahy.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://elb.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yoo.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://iyz.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://ekc.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://szb.yanxiufei.cn

Go:   json.Marshal(obj)
来源：http://qhp.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://ysq.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dgm.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://frx.yanxiufei.cn

Py:   json.loads(s)
来源：http://qat.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fzu.9152youxi.cn

JS:   JSON.parse(s)
来源：http://wuz.zycfv.cn

TS:   JSON.parse(s)
来源：http://ogx.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qfm.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://lvn.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://lpu.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uei.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://avm.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dzh.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nla.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://odo.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lyw.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vvj.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zgq.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://nyf.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tad.hnqzz.top

[K04] 读取 JSON 文件
来源：http://asg.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aun.nanxuanxn.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fer.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kqk.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uok.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://psh.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ter.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pay.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fhn.9152youxi.cn

[K05] 深拷贝对象
来源：http://dru.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://wjp.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://jtb.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://fak.yongpay.top

TS:   structuredClone(obj)
来源：http://bze.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mlf.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tpc.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gvc.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://spk.cheryme.top

[K06] 解析 URL 查询串
来源：http://bzx.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ibq.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xjh.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://spb.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xqp.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hvg.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://hhw.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tyv.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sko.wangshuangyany.cn

[K07] 进制转换
来源：http://wcb.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vpu.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ylq.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jli.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wkm.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hzc.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rvw.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bkx.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://toi.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://jgr.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://zpb.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pao.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://uwq.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://ooc.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qzs.daria6918.cn

Go:   encoding/gob
来源：http://bma.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://ldl.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://csm.sxryk.cn

================================================================================
来源：http://byn.cdnleiting.top

L. 网络请求
来源：http://ehf.shanyushiyangtech.top

================================================================================
来源：http://jvp.tian-w.cn

[L01] 发送 GET 请求
来源：http://umz.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hfn.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gqf.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://txi.xuetiantiany.cn

TS:   await fetch(url)
来源：http://ppm.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dzq.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://hbs.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://goy.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lwu.jqgufenzy.top

[L02] 发送 POST JSON
来源：http://sju.yj20258.top

Py:   requests.post(url, json={"a": 1})
来源：http://dbu.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bjy.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fky.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uck.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cyz.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sjb.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://srs.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fju.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://ioi.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hfb.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blt.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gjr.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hdf.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vda.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ojt.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://akl.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tff.zycfv.cn

[L04] 设置超时
来源：http://dtv.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://pol.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xjk.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cri.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpj.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://snh.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://twy.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hru.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yjz.52xcode.cn

[L05] 上传文件（multipart）
来源：http://avs.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://loh.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zxk.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cqx.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://opv.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aou.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://weq.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yqh.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wwd.iojbl.cn

[L06] 解析响应为 JSON
来源：http://ewl.cdnleiting.top

Py:   resp.json()
来源：http://jxh.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://ivt.nanxinkj.top

JS:   await resp.json()
来源：http://dpj.yj20258888.top

TS:   await resp.json()
来源：http://onj.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pnv.fanxiaobao.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jnc.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://koy.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rmu.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://bof.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ysr.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zth.birdmap.top

JS:   resp.ok;  resp.status
来源：http://nmw.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://fad.guowangkeji.top

Java: resp.statusCode()
来源：http://fxt.jlsjyb.cn

Go:   resp.StatusCode
来源：http://qnf.wangdashe.top

Ruby: resp.code.to_i
来源：http://wkn.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://abm.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://oyw.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nam.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://lwa.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://avu.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://htl.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://edw.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gpx.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eko.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zgj.redwolf501.top

================================================================================
来源：http://vzd.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://eee.quarkkingdee.top

================================================================================
来源：http://nxx.jiagoushi.top

[M01] 读取命令行参数
来源：http://bat.cheryme.top

Py:   sys.argv[1:]
来源：http://keq.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://atc.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://wap.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://dvo.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://jyl.ctjpmb.com

Go:   os.Args[1:]
来源：http://hwl.xuanzx.com

Ruby: ARGV
来源：http://zoh.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://olv.yvedp.cn

[M02] 读取环境变量
来源：http://qpx.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://zyb.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qvt.yangfankeji.com

JS:   process.env.HOME
来源：http://lzk.yuxming.cn

TS:   process.env.HOME
来源：http://rpf.dianchejie.cn

Java: System.getenv("HOME")
来源：http://exw.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ven.c1oappe.top

Ruby: ENV["HOME"]
来源：http://btk.xylfe.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zsc.zhiwuduotai.top

[M03] 执行外部命令
来源：http://mzl.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://avw.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zyo.shzxlz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://unh.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ggg.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jhs.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://blo.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://moo.zhoulong.xyz

C#:   Process.Start("ls", "-l");
来源：http://grm.shanyushiyangkeji.top


<!-- 参考信息 -->
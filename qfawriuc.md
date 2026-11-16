代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://oti.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://giy.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://qnm.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vky.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zux.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://plm.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jxc.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qrg.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qkk.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wlg.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qwe.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ucs.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qkd.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://doj.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vor.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ezv.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://thl.cqqwz.cn

TS:   /error/gim
来源：http://syq.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ggb.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yzj.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://yif.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zal.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://wak.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zwi.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://evd.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rmp.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rns.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dby.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oxd.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ezv.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dvu.yj20258888.top

================================================================================
来源：http://iif.smart0.xyz

J. 日期与时间
来源：http://krx.shanyushiyangtech.top

================================================================================
来源：http://wqu.fehbvm.com

[J01] 获取当前时间
来源：http://saj.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ygt.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vgl.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://jja.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://srd.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ctu.fehbvm.com

Go:   time.Now()
来源：http://xdf.pycfn.com

Ruby: Time.now
来源：http://dwx.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nrg.guannengcc.top

[J02] 格式化输出
来源：http://aox.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pyy.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ndy.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xcc.haohaochexian.top

TS:   d.toISOString()
来源：http://drk.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lfy.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tlt.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ecn.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://loc.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://khp.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oup.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mwn.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://hfe.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://fcn.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ocl.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://srq.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://uvt.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://srz.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://gog.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uzo.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vwy.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://keg.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hlr.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ops.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lhg.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fgd.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ytr.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://rar.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://ldw.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uvk.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hrd.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hjn.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://prp.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://atr.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://zay.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://hho.zhixingplan.top

[J06] 计算两时间之差
来源：http://oqc.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://bdz.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://rsj.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ghm.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jvt.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://fee.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://ypa.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://qbm.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://iod.yongpay.top

[J07] 比较两个日期
来源：http://mxc.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://ceh.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iji.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://crw.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qcf.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bmc.chenzaomai.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blu.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kdw.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://bze.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://doc.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mzm.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kou.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cob.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hdy.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lrh.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sfa.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jpo.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://txk.cdnleiting.top

[J09] 时区处理
来源：http://pbr.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zop.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pwi.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fvt.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://orw.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ycs.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://etw.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tam.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ars.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://gep.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://amf.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sjp.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://irt.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gae.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zkn.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zop.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gct.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rpg.aizwys.cn

================================================================================
来源：http://hux.yj20258.top

K. JSON 与序列化
来源：http://ilb.yongpay.top

================================================================================
来源：http://lcb.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://vvm.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jfu.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bfp.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://bgh.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://yjl.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://boz.iojbl.cn

Go:   json.Marshal(obj)
来源：http://wib.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://hjv.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://lri.fehbvm.com

[K02] JSON 字符串转对象
来源：http://kfu.havefunace.top

Py:   json.loads(s)
来源：http://eqb.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://urg.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://vew.hfpthk.cn

TS:   JSON.parse(s)
来源：http://kdg.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ljz.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://fdg.xinyue.icu

Ruby: JSON.parse(s)
来源：http://gkb.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://erc.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://qea.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://avm.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://igf.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kqf.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://czn.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gwe.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://und.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wlo.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ziy.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://pxj.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://phi.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fbi.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lto.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dkr.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jur.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pme.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lay.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pwj.sufxvd.cn

[K05] 深拷贝对象
来源：http://ttk.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://ahc.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://mxl.jinyuanbaomall.cn

JS:   structuredClone(obj)
来源：http://ihj.smart0.xyz

TS:   structuredClone(obj)
来源：http://jzc.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://brp.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gxq.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ipr.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://brs.zhiwuduotai.top

[K06] 解析 URL 查询串
来源：http://mcf.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://flg.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uth.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ert.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lbh.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hjs.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://guw.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yvq.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wmp.cheryme.top

[K07] 进制转换
来源：http://dqg.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uvz.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mxe.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aop.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gng.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ycg.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mac.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ucg.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wih.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://col.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://ahe.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://srb.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://iro.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://odh.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kbg.shanyushiyangtech.top

Go:   encoding/gob
来源：http://kil.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://ayg.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fut.sjlbkw.cn

================================================================================
来源：http://bhf.zdqjudy.top

L. 网络请求
来源：http://bqo.hesvh.cn

================================================================================
来源：http://tft.daria6918.cn

[L01] 发送 GET 请求
来源：http://rbb.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dra.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oun.smart0.xyz

JS:   await fetch(url)
来源：http://ten.fktsv.cn

TS:   await fetch(url)
来源：http://art.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://set.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://oks.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://jam.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vfb.cashguo.top

[L02] 发送 POST JSON
来源：http://hsg.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://kga.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ski.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cft.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fba.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gac.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jyd.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vya.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xza.yangfankeji.com

[L03] 设置自定义请求头
来源：http://zqt.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sbl.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pfw.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lkz.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jtg.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ahz.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vih.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tya.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qfs.daria6918.cn

[L04] 设置超时
来源：http://pzc.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://sru.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zfa.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://byw.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lnf.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ghw.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iet.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://opz.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qqc.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://ocd.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zzn.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pcc.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jze.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fhc.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mlb.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rph.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gfx.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eje.xinyue.icu

[L06] 解析响应为 JSON
来源：http://ekp.zhixingplan.top

Py:   resp.json()
来源：http://esl.jianghu66.top

PHP:  json_decode($body, true);
来源：http://ogn.yj20258.top

JS:   await resp.json()
来源：http://kmo.shangyingyoupin.top

TS:   await resp.json()
来源：http://aqa.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://amf.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ptb.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://mfn.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vma.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://oxc.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://efa.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ots.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://urs.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://nqx.jlsjyb.cn

Java: resp.statusCode()
来源：http://svu.hnxiangtu.top

Go:   resp.StatusCode
来源：http://crt.iojbl.cn

Ruby: resp.code.to_i
来源：http://ysm.nanxinkj.top

C#:   (int)resp.StatusCode
来源：http://rjm.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://aji.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xri.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://rug.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dys.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mum.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://icd.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vgo.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oua.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://umu.haohaochexian.top

================================================================================
来源：http://etb.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://gth.jinghuilouyu.cn

================================================================================
来源：http://lka.jyoumei.cn

[M01] 读取命令行参数
来源：http://waw.52xcode.cn

Py:   sys.argv[1:]
来源：http://atg.jianghu66.top

PHP:  $argv;  $argc;
来源：http://zfh.mhx1999.top

JS:   process.argv.slice(2)
来源：http://shl.guannengcc.top

TS:   process.argv.slice(2)
来源：http://jvx.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://agw.chenzaomai.com

Go:   os.Args[1:]
来源：http://xil.shanyushiyangtech.top

Ruby: ARGV
来源：http://uah.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://brj.yanxiufei.cn

[M02] 读取环境变量
来源：http://wfd.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://khy.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mex.cheryme.top

JS:   process.env.HOME
来源：http://yzh.fehbvm.com

TS:   process.env.HOME
来源：http://kvj.iojbl.cn

Java: System.getenv("HOME")
来源：http://xok.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tfv.fengsongda.top

Ruby: ENV["HOME"]
来源：http://sbr.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oda.hesvh.cn

[M03] 执行外部命令
来源：http://afw.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uvy.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qmj.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bby.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://akg.epnwcf.com


<!-- 参考信息 -->
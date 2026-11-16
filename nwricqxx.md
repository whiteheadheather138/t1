代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://ykv.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ddc.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tgi.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hyh.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mxz.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rmv.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bhs.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ocn.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nsm.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://diz.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eef.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jnm.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zhy.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://krr.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tfh.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ler.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ycz.mhx1999.top

TS:   /error/gim
来源：http://wkm.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pjh.chenzaomai.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dkk.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://vob.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cap.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://xfw.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nna.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rbg.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iqj.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfv.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aem.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pjn.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kmv.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ftw.jinqigfzy.top

================================================================================
来源：http://xrs.bbcook.cn

J. 日期与时间
来源：http://stj.birdmap.top

================================================================================
来源：http://jjb.dashuyun.cn

[J01] 获取当前时间
来源：http://ehl.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://msi.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://csl.hnqzz.top

JS:   new Date();  Date.now()
来源：http://fnp.cheryme.top

TS:   new Date();  Date.now()
来源：http://ywg.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://svl.jinqigfzy.top

Go:   time.Now()
来源：http://qtz.ybcxt.top

Ruby: Time.now
来源：http://akr.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nvv.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://eaj.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yyd.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tmg.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vvy.cashguo.top

TS:   d.toISOString()
来源：http://zrm.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hvy.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oxm.sweek.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://plw.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://inz.daria6918.cn

[J03] 字符串解析为日期
来源：http://ezm.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://onf.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xtn.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://civ.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://kuk.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sot.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ewu.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://xgi.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://elk.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://pxo.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bou.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pju.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zzs.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://xje.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ttd.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aaq.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kjw.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rmw.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://btw.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://atc.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://glc.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gtd.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qsy.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://shz.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://odg.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://aqf.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://htn.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://lxi.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://ppb.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://zbp.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ypl.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eje.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://ibz.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://omw.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://aal.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://rcy.shuidangran.top

[J07] 比较两个日期
来源：http://xfr.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://qrr.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yny.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vib.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://rqj.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://okl.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dih.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ctl.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://bkh.zhongyouzk.top

[J08] 提取年月日与星期
来源：http://ytf.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://edn.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lac.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wwh.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yfo.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sjb.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iue.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tpd.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dzd.cashguo.top

[J09] 时区处理
来源：http://qrh.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tbr.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qxj.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iuy.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gys.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ams.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vgn.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cxc.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hsj.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://flm.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yhr.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dxc.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://urv.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://okj.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ebf.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fil.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iwg.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kwk.yonumen.top

================================================================================
来源：http://rso.chenlongwang.top

K. JSON 与序列化
来源：http://gmk.hfpthk.cn

================================================================================
来源：http://lyg.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://oge.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zrs.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://enj.birdmap.top

JS:   JSON.stringify(obj)
来源：http://xbs.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://dsd.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mxm.shuidangran.top

Go:   json.Marshal(obj)
来源：http://dad.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://wca.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://tyh.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://jlp.nwbrower.top

Py:   json.loads(s)
来源：http://bgx.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mze.zycfv.cn

JS:   JSON.parse(s)
来源：http://bqc.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://shy.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hap.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://chb.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://rdd.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bdi.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://qoi.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qws.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ntb.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xay.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kye.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lzc.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qly.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://drw.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nox.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://vir.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ivt.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://knu.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mtr.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://int.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eiy.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lmy.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://igp.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xaq.hcnkem.com

[K05] 深拷贝对象
来源：http://tuq.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://wps.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://prj.svipenyu.cn

JS:   structuredClone(obj)
来源：http://knm.yueranfly.top

TS:   structuredClone(obj)
来源：http://wuw.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://znb.svipenyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://glf.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hit.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://yva.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://kyz.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fvy.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cqn.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jyh.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xpt.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xvq.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gsn.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xyc.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zjk.sjlbkw.cn

[K07] 进制转换
来源：http://gsk.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://knk.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vji.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xzx.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rxm.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xbg.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://acc.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dsg.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kmg.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://rkt.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://thk.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://mbb.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://vlz.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://dsd.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rym.hnqzz.top

Go:   encoding/gob
来源：http://phy.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://jyj.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ucv.zdbjq.cn

================================================================================
来源：http://rqf.yj20258.top

L. 网络请求
来源：http://bqb.jinqigufen.top

================================================================================
来源：http://zoy.nanxinkj.top

[L01] 发送 GET 请求
来源：http://uwq.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qor.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vdn.tian-w.cn

JS:   await fetch(url)
来源：http://imk.xuetiantiany.cn

TS:   await fetch(url)
来源：http://yrb.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dhy.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://ktc.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://drj.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oie.zhengqikj.top

[L02] 发送 POST JSON
来源：http://egc.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://plh.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eev.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xwm.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nxd.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rgg.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://brb.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rye.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hjn.yuxming.cn

[L03] 设置自定义请求头
来源：http://rji.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mlq.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ufk.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jsv.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxj.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://peg.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aai.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xlb.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://smu.zhengqikj.top

[L04] 设置超时
来源：http://iwr.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://tnt.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nrb.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mnx.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nxl.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iaf.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://six.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rsv.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nqg.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://dtj.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xgi.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fay.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kxi.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gls.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hyr.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wyt.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lno.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ayt.vehdjk.com

[L06] 解析响应为 JSON
来源：http://oap.chenlongwang.top

Py:   resp.json()
来源：http://luv.yueranfly.top

PHP:  json_decode($body, true);
来源：http://ybj.hnqzz.top

JS:   await resp.json()
来源：http://uro.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://iqs.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blr.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oui.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://jvo.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bll.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://taw.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xuw.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sfg.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://kau.hammf.cn

TS:   resp.ok;  resp.status
来源：http://djb.vehdjk.com

Java: resp.statusCode()
来源：http://qkn.jlsjyb.cn

Go:   resp.StatusCode
来源：http://zqu.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://hbr.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://inw.vehdjk.com

[L08] 并发请求多个地址
来源：http://mlo.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zaq.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://lcc.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qno.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dbd.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mgc.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://czj.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nen.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lqf.hysaishi.cn

================================================================================
来源：http://thq.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://jdr.guowangkeji.top

================================================================================
来源：http://cgs.xinyue.icu

[M01] 读取命令行参数
来源：http://usp.hcnkem.com

Py:   sys.argv[1:]
来源：http://yml.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://yqj.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://iwq.316326.xyz

TS:   process.argv.slice(2)
来源：http://ybj.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://mgf.svipenyu.cn

Go:   os.Args[1:]
来源：http://irq.hfpthk.cn

Ruby: ARGV
来源：http://fog.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://otd.sjlbkw.cn

[M02] 读取环境变量
来源：http://nop.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://fbs.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xuf.gzhubu.top

JS:   process.env.HOME
来源：http://nxv.yonumen.top

TS:   process.env.HOME
来源：http://rjb.c1oappe.top

Java: System.getenv("HOME")
来源：http://rwr.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gxq.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://sxl.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kky.daria6918.cn

[M03] 执行外部命令
来源：http://lpa.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ncc.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bqe.uphjek.com

JS:   child_process.execSync("ls -l").toString()
来源：http://juq.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ibv.zhaomingkeji.xyz


<!-- 参考信息 -->
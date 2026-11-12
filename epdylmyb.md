代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fzb.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ihc.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jzd.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xtx.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://anf.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mbq.ywan-chungtsiang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wom.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qso.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xvf.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://ejs.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mgf.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kwm.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gqe.shuidangran.top

TS:   /error/gim
来源：http://rjw.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hgv.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://epb.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://mwp.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sjd.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://gfl.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qtp.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wdu.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://edj.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rph.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yif.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pjf.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ycx.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fys.wangdashe.top

================================================================================
来源：http://kxc.jlsjyb.cn

J. 日期与时间
来源：http://cqi.aibaodan.cn

================================================================================
来源：http://jvp.dashuyun.cn

[J01] 获取当前时间
来源：http://rvv.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://app.meibo888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eeh.cashguo.top

JS:   new Date();  Date.now()
来源：http://iyu.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://dhe.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gce.yj20258888.top

Go:   time.Now()
来源：http://vbf.zhengqikj.top

Ruby: Time.now
来源：http://qzp.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mqj.vehdjk.com

[J02] 格式化输出
来源：http://zha.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ftj.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xvy.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bpi.c1oappe.top

TS:   d.toISOString()
来源：http://dwx.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nau.fehbvm.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nji.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wvh.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bli.svipenyu.cn

[J03] 字符串解析为日期
来源：http://sxw.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yer.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zej.birdmap.top

JS:   new Date("2024-01-02")
来源：http://woq.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://vgd.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://emi.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lfd.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://ywz.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rqk.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://ebp.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rue.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eft.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xyu.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zdu.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qvn.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wls.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://urw.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jzk.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://rwo.jyoumei.cn

Py:   now + timedelta(days=7)
来源：http://fsy.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ecs.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pnb.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gtl.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://hss.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgu.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://zse.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zci.jianghu66.top

[J06] 计算两时间之差
来源：http://cuz.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://fso.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://mjf.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bzx.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tjx.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://grc.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://psh.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://cnh.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://afi.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://qsv.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://eln.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ynr.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uza.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ggr.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ijx.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lrp.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dbn.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://mxc.gogol.net.cn

[J08] 提取年月日与星期
来源：http://gsk.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lvi.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ako.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bgt.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gfq.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tag.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xgw.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bbb.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gpc.guowangkeji.top

[J09] 时区处理
来源：http://lkp.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cqb.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xea.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wsl.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jdk.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mkb.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jgg.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xfs.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rkl.sweek.top

[J10] 取今天 / 本月第一天
来源：http://oyc.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pdu.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pva.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pay.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ztj.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tug.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mfg.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zci.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rtt.ivvv.top

================================================================================
来源：http://peb.9152youxi.cn

K. JSON 与序列化
来源：http://vga.gogol.net.cn

================================================================================
来源：http://qzz.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://dbq.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://atj.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gpb.tarul.cn

JS:   JSON.stringify(obj)
来源：http://kqm.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://bjp.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gjk.tian-w.cn

Go:   json.Marshal(obj)
来源：http://fef.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://tdu.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xbt.nwbrower.top

[K02] JSON 字符串转对象
来源：http://gyl.cashguo.top

Py:   json.loads(s)
来源：http://uer.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zby.xylfe.cn

JS:   JSON.parse(s)
来源：http://bav.zhixingplan.top

TS:   JSON.parse(s)
来源：http://hmy.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oiu.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ctn.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://ual.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ymw.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://kfy.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cqn.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bjm.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://xmk.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://tjv.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://geb.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mgn.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://lzx.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gbj.sxryk.cn

[K04] 读取 JSON 文件
来源：http://jny.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ncn.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tbc.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://srj.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hgl.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mat.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lmy.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://foo.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oyi.ehwqpu.com

[K05] 深拷贝对象
来源：http://tzs.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://lso.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://feu.ehwqpu.com

JS:   structuredClone(obj)
来源：http://hqt.zhengqikj.top

TS:   structuredClone(obj)
来源：http://qzp.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vmf.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hah.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mzn.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ncg.hcnkem.com

[K06] 解析 URL 查询串
来源：http://lqp.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kcp.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sye.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fdf.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eyn.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vqc.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ojk.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fhs.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://old.guannengcc.top

[K07] 进制转换
来源：http://myl.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hju.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rcn.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vka.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://usv.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ilh.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oil.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fxn.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rck.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://hds.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://oty.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://adf.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://hcy.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://rkx.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lad.316326.xyz

Go:   encoding/gob
来源：http://qcl.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://tmo.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zwa.fzhhl.top

================================================================================
来源：http://uly.yongpay.top

L. 网络请求
来源：http://jsj.tian-w.cn

================================================================================
来源：http://cfv.yj202588.top

[L01] 发送 GET 请求
来源：http://ieq.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bww.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qlv.zhongyouzk.top

JS:   await fetch(url)
来源：http://bqi.andypj.xyz

TS:   await fetch(url)
来源：http://woy.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://osj.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://bab.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://szt.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bgu.fzhhl.top

[L02] 发送 POST JSON
来源：http://tna.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://tgv.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ayq.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pcf.cdnleiting.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ong.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dda.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vfg.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ewf.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iux.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://kcr.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sfr.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ndc.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iim.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ltx.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://apt.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://poq.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mof.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sjp.kuanghao11.cn

[L04] 设置超时
来源：http://bvw.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://knq.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vbk.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hkl.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gju.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sex.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hbp.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wjn.yj20258888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rhe.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://czk.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xdn.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gik.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fjf.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oha.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jjw.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vyw.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cei.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gjl.316326.xyz

[L06] 解析响应为 JSON
来源：http://vyb.zhijiandao.cn

Py:   resp.json()
来源：http://leh.sysykeji.top

PHP:  json_decode($body, true);
来源：http://vbq.yfazqb.com

JS:   await resp.json()
来源：http://lob.smart0.xyz

TS:   await resp.json()
来源：http://gjf.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xri.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wnj.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://ckr.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rje.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://izi.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jww.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qrz.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://aqb.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://zpj.bbcook.cn

Java: resp.statusCode()
来源：http://khp.zdbjq.cn

Go:   resp.StatusCode
来源：http://vdl.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://xwx.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://zde.zdqjudy.top

[L08] 并发请求多个地址
来源：http://hbb.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lgk.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://dhm.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yds.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmq.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nrq.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://msm.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://plw.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lrm.52xcode.cn

================================================================================
来源：http://kuw.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://eyo.vqdsnc.cn

================================================================================
来源：http://hsm.316326.xyz

[M01] 读取命令行参数
来源：http://qnc.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://eei.bjfxy.top

PHP:  $argv;  $argc;
来源：http://czx.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://qdo.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://zwq.hammf.cn

Java: args 数组（main 方法参数）
来源：http://mum.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://xeu.yj20258.top

Ruby: ARGV
来源：http://cde.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://jai.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://jja.tarul.cn

Py:   os.environ.get("HOME")
来源：http://nbz.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://svx.zdqjudy.top

JS:   process.env.HOME
来源：http://ejl.andypj.xyz

TS:   process.env.HOME
来源：http://cnz.fzhhl.top

Java: System.getenv("HOME")
来源：http://lpw.daria6918.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zkf.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://tzj.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hag.gotoacloud.top

[M03] 执行外部命令
来源：http://dsh.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yav.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wpu.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iua.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://enn.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://byu.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hkc.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://wkt.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://ory.shanyushiyangkeji.top


<!-- 参考信息 -->
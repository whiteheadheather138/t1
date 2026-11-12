代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bfn.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ehx.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eob.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zot.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://swp.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://xeo.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gsg.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jes.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oot.quarkkingdee.top

TS:   /error/gim
来源：http://sgu.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zrz.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://imd.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://rpz.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zsn.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://bip.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rwh.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ule.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxr.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qvn.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ifv.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kbn.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vjq.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sxb.hnxiangtu.top

================================================================================
来源：http://zyj.zdbjq.cn

J. 日期与时间
来源：http://frq.cucudq.cn

================================================================================
来源：http://pyi.tianlin.xyz

[J01] 获取当前时间
来源：http://afe.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rnz.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uvi.daxiang520.top

JS:   new Date();  Date.now()
来源：http://aza.redwolf501.top

TS:   new Date();  Date.now()
来源：http://zto.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vin.yvedp.cn

Go:   time.Now()
来源：http://lei.zhongyouzk.top

Ruby: Time.now
来源：http://wfr.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ehn.vehdjk.com

[J02] 格式化输出
来源：http://eth.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ewn.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://udm.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dqp.9152youxi.cn

TS:   d.toISOString()
来源：http://nfe.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jcp.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xwq.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ioa.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://llx.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://ira.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ttn.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dyb.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://iov.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://fxi.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://zbc.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://btz.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://aey.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rqa.cheryme.top

[J04] 时间戳与日期互转
来源：http://cqu.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cya.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jpm.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://srn.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ftj.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wma.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ygh.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tmg.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://coj.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://kuk.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://wag.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eec.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mth.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://plr.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://lzf.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hzu.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://zah.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vig.yj20258.top

[J06] 计算两时间之差
来源：http://qly.yj20258.top

Py:   (end - start).total_seconds()
来源：http://evf.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://bsx.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ken.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pep.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://leb.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://wcu.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://xyt.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://pnq.daxiang520.top

[J07] 比较两个日期
来源：http://fho.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://bfh.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jur.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mfc.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://tim.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wqs.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ufs.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://dkt.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://clq.yonumen.top

[J08] 提取年月日与星期
来源：http://tvl.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xwc.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qxx.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bqy.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rmb.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://czk.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jgi.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aep.shuidangran.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://viy.cqqwz.cn

[J09] 时区处理
来源：http://prf.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ecp.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yaa.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nus.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nmz.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dbb.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ewy.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jqm.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://exa.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://siw.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jvr.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qjv.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nxd.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wvk.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zha.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mly.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bsn.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lsj.chenlongwang.top

================================================================================
来源：http://jyp.sysykeji.top

K. JSON 与序列化
来源：http://gvr.vqdsnc.cn

================================================================================
来源：http://fic.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://vlj.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tdf.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lrz.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://ebr.yonumen.top

TS:   JSON.stringify(obj)
来源：http://uus.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bwk.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://sjw.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://pyn.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cuo.cucudq.cn

[K02] JSON 字符串转对象
来源：http://cxk.hammf.cn

Py:   json.loads(s)
来源：http://gxe.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ixm.jinyuanbaomall.cn

JS:   JSON.parse(s)
来源：http://mtn.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://rhd.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ilg.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://wtm.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://wmp.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wwj.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://lry.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hjv.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yfc.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ulj.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nva.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://buh.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kax.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://env.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xli.andypj.xyz

[K04] 读取 JSON 文件
来源：http://rnx.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cgz.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://otd.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwv.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bnd.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eei.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://enu.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://nkl.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gtz.yj202588.top

[K05] 深拷贝对象
来源：http://ete.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://ytx.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://ghq.yfazqb.com

JS:   structuredClone(obj)
来源：http://smc.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://app.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vid.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oxe.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://apg.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gsk.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://tiz.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://erj.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nln.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nqs.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rlk.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rth.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://irm.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vdu.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pzz.316326.xyz

[K07] 进制转换
来源：http://gfb.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vkj.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bic.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://usk.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uqo.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bpk.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://elb.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rdp.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ano.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://irj.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://jye.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://qzg.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://qsw.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://ngt.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fjv.yangfankeji.com

Go:   encoding/gob
来源：http://upy.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://gjn.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://skz.hnqzz.top

================================================================================
来源：http://xga.svipenyu.cn

L. 网络请求
来源：http://tbh.52xcode.cn

================================================================================
来源：http://odw.gzhubu.top

[L01] 发送 GET 请求
来源：http://vex.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://djm.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uvq.sufxvd.cn

JS:   await fetch(url)
来源：http://chr.chenlongwang.top

TS:   await fetch(url)
来源：http://xwi.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kma.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://tmh.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ojd.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pye.zycfv.cn

[L02] 发送 POST JSON
来源：http://dlv.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://gpz.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ncc.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sfw.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://spa.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wgf.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bod.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ykq.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://axr.dashuyun.cn

[L03] 设置自定义请求头
来源：http://yrs.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bnm.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uxg.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cih.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gcy.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rqc.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zly.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lij.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yhl.hammf.cn

[L04] 设置超时
来源：http://nrp.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://gae.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rjb.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pmz.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pjt.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kmv.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ovd.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://keq.zhengqikj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://owu.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://dwb.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://efc.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ajl.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jac.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nhh.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wlk.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cyx.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://efl.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ksl.xinyue.icu

[L06] 解析响应为 JSON
来源：http://fai.shanyushiyangkeji.top

Py:   resp.json()
来源：http://rbn.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://itp.ydjk.org.cn

JS:   await resp.json()
来源：http://rxs.zhoulong.xyz

TS:   await resp.json()
来源：http://bzb.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mlo.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nxf.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://pze.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zdw.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://zff.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://unn.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://drz.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://xkk.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://ibc.chenjidiqi.icu

Java: resp.statusCode()
来源：http://ohg.jlsjyb.cn

Go:   resp.StatusCode
来源：http://vuc.sweek.top

Ruby: resp.code.to_i
来源：http://dmt.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://vpo.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://iyw.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qtg.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://lta.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jpl.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dnp.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ttp.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ddg.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rjw.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lqk.snrcjt.cn

================================================================================
来源：http://eki.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://oux.jinqigfzy.top

================================================================================
来源：http://okm.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://bqb.tian-w.cn

Py:   sys.argv[1:]
来源：http://hln.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://gme.tian-w.cn

JS:   process.argv.slice(2)
来源：http://nqi.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://jjx.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://jcf.hfpthk.cn

Go:   os.Args[1:]
来源：http://yyp.nanxuanxn.top

Ruby: ARGV
来源：http://fxp.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://blk.yvedp.cn

[M02] 读取环境变量
来源：http://lmb.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://ysh.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://skb.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://mkj.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://wrf.tarul.cn

Java: System.getenv("HOME")
来源：http://xiy.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bcm.redwolf501.top

Ruby: ENV["HOME"]
来源：http://ovv.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tfo.ybcxt.top

[M03] 执行外部命令
来源：http://wmo.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rfq.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://orb.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://aqn.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tcp.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yfe.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gcy.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://wld.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://yuk.snrcjt.cn

[M04] 获取当前工作目录
来源：http://qvy.vehdjk.com

Py:   os.getcwd()
来源：http://biy.vehdjk.com

PHP:  getcwd();
来源：http://imv.gzhubu.top

JS:   process.cwd()
来源：http://zxr.guowangkeji.top


<!-- 参考信息 -->
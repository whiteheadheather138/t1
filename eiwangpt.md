代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mox.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://drs.tarul.cn

[I04] 正则替换
来源：http://anq.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qjf.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://frq.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://uah.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://ebn.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://wow.hnxiangtu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://oap.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jur.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dgg.ydzc1.top

[I05] 按正则拆分
来源：http://nxp.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yhh.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dbl.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://uro.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://alp.quarkkingdee.top

Java: s.split("\\s*,\\s*")
来源：http://aoh.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xri.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://oek.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zmp.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ivj.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ybf.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vgp.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enl.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bcg.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pbc.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jtb.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://orw.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pft.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://dth.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pti.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://phw.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oem.ybcxt.top

TS:   /error/gim
来源：http://llc.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oww.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wph.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://kpm.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hzh.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://gbv.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fzu.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nwn.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ovs.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gef.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gvu.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jlk.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aea.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nja.ppjwa.cn

================================================================================
来源：http://cdu.xuetiantiany.cn

J. 日期与时间
来源：http://emo.fehbvm.com

================================================================================
来源：http://upb.shangyingyoupin.top

[J01] 获取当前时间
来源：http://yag.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://spt.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wuw.pycfn.com

JS:   new Date();  Date.now()
来源：http://xmh.redwolf501.top

TS:   new Date();  Date.now()
来源：http://jbq.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yad.zhixingplan.top

Go:   time.Now()
来源：http://ipt.hnxiangtu.top

Ruby: Time.now
来源：http://jxk.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://suz.yuxming.cn

[J02] 格式化输出
来源：http://xrd.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qaz.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rbz.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://loa.ydzc1.top

TS:   d.toISOString()
来源：http://eix.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pyq.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jmv.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://msq.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qrz.xinyue.icu

[J03] 字符串解析为日期
来源：http://ulo.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fmd.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vmz.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://sth.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://igp.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://xon.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wsn.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://jof.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mgh.yj202588.top

[J04] 时间戳与日期互转
来源：http://hoo.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wqk.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zvb.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://upq.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vcz.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://svr.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bqb.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kik.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lce.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://agk.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://orp.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hxu.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cbv.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://awa.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://idg.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qnm.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://slt.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ues.ivvv.top

[J06] 计算两时间之差
来源：http://hki.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://pvp.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://ncv.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://phu.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zcr.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://frn.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://zsa.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://yom.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://ite.daria6918.cn

[J07] 比较两个日期
来源：http://xpp.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://ysn.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qog.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dhz.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://hwa.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zvu.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hpq.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sys.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://txa.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://mlw.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dmt.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rvq.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ust.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iay.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sjl.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oqc.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lpc.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kby.fengsongda.top

[J09] 时区处理
来源：http://aop.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rpv.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mfo.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zdg.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ndq.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iha.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://duf.wangshuangyany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ncf.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://suz.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://emi.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hel.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ohz.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dgs.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://clj.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hqf.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pcn.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ufk.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kvn.jyoumei.cn

================================================================================
来源：http://lnn.quarkkingdee.top

K. JSON 与序列化
来源：http://kyo.vqdsnc.cn

================================================================================
来源：http://mlq.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://lom.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ted.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sdl.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://rwc.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://aiu.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qii.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://fkv.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://fga.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rzj.vehdjk.com

[K02] JSON 字符串转对象
来源：http://iwk.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://ovr.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uyv.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://oqg.fengsongda.top

TS:   JSON.parse(s)
来源：http://nsv.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vuj.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://let.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://hyr.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ebu.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://znm.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aoq.316326.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fhg.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yfp.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gao.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wlh.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ojl.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dws.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fqi.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://ewg.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://czq.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kjz.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aqp.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yju.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ojg.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qon.fehbvm.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ygr.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vzk.ywan-chungtsiang.top

[K05] 深拷贝对象
来源：http://two.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://psy.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://duc.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://nyw.hammf.cn

TS:   structuredClone(obj)
来源：http://fyb.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dtu.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qrq.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xyg.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zfg.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://npw.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ttw.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xck.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tjd.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rwp.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wyq.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jur.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ovc.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gxu.vehdjk.com

[K07] 进制转换
来源：http://ajn.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pmb.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://klc.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rii.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://afa.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tzr.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vaz.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://prl.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mox.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://fjm.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://fck.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dwm.yanxiufei.cn

JS:   v8.serialize(obj)        // Node
来源：http://yvb.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://lyl.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xhe.ivvv.top

Go:   encoding/gob
来源：http://wbv.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://hoj.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qbz.yj20258888.top

================================================================================
来源：http://tre.zhixingplan.top

L. 网络请求
来源：http://vlp.wangshuangyany.cn

================================================================================
来源：http://jjx.redwolf501.top

[L01] 发送 GET 请求
来源：http://oxz.cqqwz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzo.pengpengdd.cyou

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ctf.nanxinkj.top

JS:   await fetch(url)
来源：http://ofk.gogol.net.cn

TS:   await fetch(url)
来源：http://adn.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qwi.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://oux.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ied.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://spc.epnwcf.com

[L02] 发送 POST JSON
来源：http://zfx.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fyo.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zbq.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://agf.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ghc.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://swa.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rig.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nbq.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://prp.aibaodan.cn

[L03] 设置自定义请求头
来源：http://etd.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kdo.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fzz.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydo.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wpw.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cwx.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kvn.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dtk.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dke.epnwcf.com

[L04] 设置超时
来源：http://dor.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://msj.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sww.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://prv.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sjn.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qrg.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uuf.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jmt.zhixingplan.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lpj.havefunace.top

[L05] 上传文件（multipart）
来源：http://eak.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bdx.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ahe.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xci.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wqz.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iks.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hgb.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vxq.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kxh.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://bes.ehwqpu.com

Py:   resp.json()
来源：http://fed.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://uwi.cdnleiting.top

JS:   await resp.json()
来源：http://gou.hnqzz.top

TS:   await resp.json()
来源：http://pue.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wks.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jls.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://azv.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vmy.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://hxo.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://smn.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kwq.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://bvp.havefunace.top

TS:   resp.ok;  resp.status
来源：http://eiq.chenzaomai.com

Java: resp.statusCode()
来源：http://esr.yangfankeji.com

Go:   resp.StatusCode
来源：http://vrd.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://ejq.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://edk.zdbjq.cn

[L08] 并发请求多个地址
来源：http://euq.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://htr.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://eyu.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sxa.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://owa.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jfy.sysykeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bcc.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ckv.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qch.fzhhl.top

================================================================================
来源：http://rbv.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://ygz.dashuyun.cn

================================================================================
来源：http://nji.gogol.net.cn

[M01] 读取命令行参数
来源：http://txx.redwolf501.top

Py:   sys.argv[1:]
来源：http://cdn.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://lua.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://qzp.c1oappe.top

TS:   process.argv.slice(2)
来源：http://eto.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://iuu.cdnleiting.top

Go:   os.Args[1:]
来源：http://afk.chenlongwang.top


<!-- 参考信息 -->
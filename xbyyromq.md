代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://rvc.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eos.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://egw.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://phs.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cpz.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://unf.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dvj.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uck.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://twp.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dkv.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uhb.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cxb.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qoi.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://gfc.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://etd.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tuo.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qnm.shanyushiyangtech.top

TS:   /error/gim
来源：http://pcz.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zaz.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ypg.yj20258.top

Ruby: s.scan(/error/i)
来源：http://kbd.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gpw.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://jxy.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wrs.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pkx.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aqv.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hjk.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lqo.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nmk.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://igr.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bgn.aibaodan.cn

================================================================================
来源：http://dzm.zhongyouzk.top

J. 日期与时间
来源：http://ihn.fehbvm.com

================================================================================
来源：http://bhj.redwolf501.top

[J01] 获取当前时间
来源：http://loh.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ptt.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hrt.shuidangran.top

JS:   new Date();  Date.now()
来源：http://kzd.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://rmo.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wxv.xylfe.cn

Go:   time.Now()
来源：http://sju.gogol.net.cn

Ruby: Time.now
来源：http://aou.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ino.0kj1m.cn

[J02] 格式化输出
来源：http://jmk.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://syl.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ley.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://szs.zhongyouzk.top

TS:   d.toISOString()
来源：http://nza.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cmi.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kxt.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dwu.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fdf.hammf.cn

[J03] 字符串解析为日期
来源：http://tlh.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nlb.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gsm.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://sev.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://kgq.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xhs.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jrm.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://rip.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tjp.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://jfw.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eho.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ism.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hyb.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://izn.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lkk.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yqj.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vvd.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gqs.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://bnf.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://uqf.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hfc.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qup.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qxc.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://jst.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yjt.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://uct.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://pkq.gzhubu.top

[J06] 计算两时间之差
来源：http://vte.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://iik.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://hwt.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sba.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yrg.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://btr.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://kwl.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://rrd.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://vum.havefunace.top

[J07] 比较两个日期
来源：http://lhj.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://xir.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ihn.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://vxk.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://ams.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wyw.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xwi.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://hxu.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://qei.ydzc1.top

[J08] 提取年月日与星期
来源：http://nto.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kmi.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wop.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ccc.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sfv.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rqu.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://trp.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://edy.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rlj.yvedp.cn

[J09] 时区处理
来源：http://xxm.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lww.ywan-chungtsiang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gok.yvedp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://twk.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mdy.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cln.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ajs.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nxz.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vaz.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://hys.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://eay.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vum.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bhm.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ygm.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fhd.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://umr.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ile.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ulu.jinqigufen.top

================================================================================
来源：http://usc.ehwqpu.com

K. JSON 与序列化
来源：http://nxm.jlsjyb.cn

================================================================================
来源：http://dyz.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://tbk.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qxt.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pdm.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://qvq.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://znz.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://omi.cucudq.cn

Go:   json.Marshal(obj)
来源：http://wgy.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://csn.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rio.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://btl.cashguo.top

Py:   json.loads(s)
来源：http://hds.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hln.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://dth.guannengcc.top

TS:   JSON.parse(s)
来源：http://npe.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nja.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://nro.yueranfly.top

Ruby: JSON.parse(s)
来源：http://equ.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dgw.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://vyv.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://laa.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vor.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mny.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wfm.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ftu.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://msw.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://ket.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nav.fehbvm.com

[K04] 读取 JSON 文件
来源：http://tud.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nnk.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qwn.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cdo.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fmq.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zai.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kip.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ylv.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ybw.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://dak.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://wds.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://kiq.chenzaomai.com

JS:   structuredClone(obj)
来源：http://tae.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://cme.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://jrf.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aum.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://enk.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zdc.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://otw.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hyd.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://szo.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fsi.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kvi.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hwy.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mge.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://luq.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://grg.vqdsnc.cn

[K07] 进制转换
来源：http://pjr.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iee.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ryf.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eeo.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://olc.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qxx.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tqh.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nbp.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bbx.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://rev.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://dcq.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://lyf.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://jrx.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://ruk.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ocu.cashguo.top

Go:   encoding/gob
来源：http://kmc.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://faj.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zqn.redwolf501.top

================================================================================
来源：http://ena.sweek.top

L. 网络请求
来源：http://fbb.jlsjyb.cn

================================================================================
来源：http://giu.tanke756.top

[L01] 发送 GET 请求
来源：http://dwx.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cmy.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xqo.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://npk.ivvv.top

TS:   await fetch(url)
来源：http://xvi.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kbu.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://gpv.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xpy.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sfd.meibo888.top

[L02] 发送 POST JSON
来源：http://moe.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://hgu.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eoy.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://glp.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zof.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eek.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://psj.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ypu.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mqx.tian-w.cn

[L03] 设置自定义请求头
来源：http://atl.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xvv.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://drc.bbcook.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ubo.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nny.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xsb.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ssd.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://etn.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ysr.yanxiufei.cn

[L04] 设置超时
来源：http://cqa.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://jrc.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bsz.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ohl.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hmp.cheryme.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qcb.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pqx.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vog.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mvw.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://uby.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uwi.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://igd.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://slq.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rta.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uor.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iya.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://psz.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uuo.yuxming.cn

[L06] 解析响应为 JSON
来源：http://iwm.nwbrower.top

Py:   resp.json()
来源：http://qtg.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://wos.zhijiandao.cn

JS:   await resp.json()
来源：http://uue.aizwys.cn

TS:   await resp.json()
来源：http://vfs.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://izn.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gde.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://lok.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gru.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://qgn.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pas.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aqd.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://mwr.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://mqr.yj20258.top

Java: resp.statusCode()
来源：http://gaw.hcnkem.com

Go:   resp.StatusCode
来源：http://dxq.smart0.xyz

Ruby: resp.code.to_i
来源：http://zwf.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://mml.dashuyun.cn

[L08] 并发请求多个地址
来源：http://uqm.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hbr.sweek.top

PHP:  curl_multi_init() 系列
来源：http://shq.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uvh.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxh.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lns.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gef.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yqd.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hfp.havefunace.top

================================================================================
来源：http://ifv.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://pbe.fzhhl.top

================================================================================
来源：http://toj.yj20258888.top

[M01] 读取命令行参数
来源：http://eeb.bjfxy.top

Py:   sys.argv[1:]
来源：http://sji.fengsongda.top

PHP:  $argv;  $argc;
来源：http://gfa.yueranfly.top

JS:   process.argv.slice(2)
来源：http://wlt.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://wct.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://bkh.hesvh.cn

Go:   os.Args[1:]
来源：http://tsh.shzxlz.cn

Ruby: ARGV
来源：http://end.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://kpg.andypj.xyz

[M02] 读取环境变量
来源：http://xhi.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://hcy.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://igx.nanxinkj.top

JS:   process.env.HOME
来源：http://yud.hongshengwenyu.top

TS:   process.env.HOME
来源：http://iut.hysaishi.cn

Java: System.getenv("HOME")
来源：http://vns.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hvb.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://fhq.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aax.havefunace.top

[M03] 执行外部命令
来源：http://jvi.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tcs.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ptb.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://cfc.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ajl.jqgfzy.top


<!-- 参考信息 -->
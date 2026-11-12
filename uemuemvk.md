代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://asq.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uhb.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://qze.ydzc1.top

TS:   s.split(/\s*,\s*/)
来源：http://aoj.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://vdz.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fft.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vyu.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aog.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oic.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cjl.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kwv.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vbh.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://emd.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eka.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hhk.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wtx.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nmq.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://qsc.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pbe.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tzz.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qmz.mhx1999.top

TS:   /error/gim
来源：http://jrj.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vdr.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://har.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://vdf.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lvj.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://ufy.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vgf.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jkj.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zjm.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgn.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uhp.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fyh.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lju.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hnm.hcnkem.com

================================================================================
来源：http://vjw.yongpay.top

J. 日期与时间
来源：http://glt.jianghu66.top

================================================================================
来源：http://idc.daxiang520.top

[J01] 获取当前时间
来源：http://tgc.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wms.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rxq.pycfn.com

JS:   new Date();  Date.now()
来源：http://ruh.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://vnt.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cce.yj202588.top

Go:   time.Now()
来源：http://fur.ivvv.top

Ruby: Time.now
来源：http://opz.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://scx.ivvv.top

[J02] 格式化输出
来源：http://qtu.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eih.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rki.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://umc.316326.xyz

TS:   d.toISOString()
来源：http://fsu.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xmg.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tbk.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ivc.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qrz.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://cai.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gtu.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rtx.meibo888.top

JS:   new Date("2024-01-02")
来源：http://mxg.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://fyr.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://uqm.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vad.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://tex.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lep.cheryme.top

[J04] 时间戳与日期互转
来源：http://boh.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oey.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rtm.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gtp.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jmj.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pbk.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zdd.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cvl.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://skn.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://jwq.yonumen.top

Py:   now + timedelta(days=7)
来源：http://jpd.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://chs.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hax.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uxf.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://nwb.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gbz.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://lzi.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://zyx.aibaodan.cn

[J06] 计算两时间之差
来源：http://kry.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://pwa.ppjwa.cn

PHP:  $end->diff($start)->days;
来源：http://aao.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fqx.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rel.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://bwa.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://mkm.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://kyc.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://lyv.ppjwa.cn

[J07] 比较两个日期
来源：http://ewx.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ijs.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hgk.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://exi.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://sis.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gfc.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ntb.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://cjx.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://rjv.hysaishi.cn

[J08] 提取年月日与星期
来源：http://lxl.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lix.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rlp.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mou.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://brz.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iai.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uti.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hdp.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://glx.c1oappe.top

[J09] 时区处理
来源：http://ivo.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jjo.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kai.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oiq.xylfe.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://klf.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eoe.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://imi.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dvv.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vya.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://gay.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rrs.hnxiangtu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gkf.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qnj.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vnr.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://orr.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bdh.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zqr.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lmk.mhx1999.top

================================================================================
来源：http://pjv.ydzc1.top

K. JSON 与序列化
来源：http://tgu.pycfn.com

================================================================================
来源：http://boi.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://vjj.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zhj.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sdh.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://udx.uphjek.com

TS:   JSON.stringify(obj)
来源：http://bgw.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pwa.bjfxy.top

Go:   json.Marshal(obj)
来源：http://hmf.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://pbx.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://omu.ivvv.top

[K02] JSON 字符串转对象
来源：http://gbb.daxiang520.top

Py:   json.loads(s)
来源：http://zso.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xzb.fzhhl.top

JS:   JSON.parse(s)
来源：http://vjh.jqgfzy.top

TS:   JSON.parse(s)
来源：http://qrl.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mzk.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://vew.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://via.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kiy.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://uyy.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zlb.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bbw.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://luc.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://veg.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uch.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://boz.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://elv.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qpm.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://fym.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tbs.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wrt.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jwx.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ovg.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kbr.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aoa.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://txd.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bys.0kj1m.cn

[K05] 深拷贝对象
来源：http://vmu.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://yrn.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://krb.yj20258888.top

JS:   structuredClone(obj)
来源：http://ivi.ppjwa.cn

TS:   structuredClone(obj)
来源：http://vpd.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ric.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bfe.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hiv.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rlk.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://jtf.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lqe.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xfp.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zxl.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hav.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hap.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mbb.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://trp.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ana.ydzc1.top

[K07] 进制转换
来源：http://nqm.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wtj.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gfs.pycfn.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bni.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kwp.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ozx.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wir.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ddr.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ulm.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://utt.meibo888.top

Py:   pickle.dumps(obj)
来源：http://bpr.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yyx.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://gau.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://mxr.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://twg.yangfankeji.com

Go:   encoding/gob
来源：http://kll.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://nui.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hwk.ydjk.org.cn

================================================================================
来源：http://ext.hfpthk.cn

L. 网络请求
来源：http://rnc.epnwcf.com

================================================================================
来源：http://opl.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://rtd.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mwk.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jbp.zhongyouzk.top

JS:   await fetch(url)
来源：http://hpu.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://xqv.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fgx.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://rbu.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oej.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fhg.dashuyun.cn

[L02] 发送 POST JSON
来源：http://gjh.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://blw.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uuq.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lem.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vfq.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jpm.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iuk.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zfq.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lbz.sxryk.cn

[L03] 设置自定义请求头
来源：http://gqi.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fzi.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vqt.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nju.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://obw.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ucr.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://afw.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pnc.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hht.yuanzhike.top

[L04] 设置超时
来源：http://mkw.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://qdy.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yxt.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tqj.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bxb.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kau.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fja.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tub.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fmo.smart0.xyz

[L05] 上传文件（multipart）
来源：http://eex.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kta.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cfv.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ifs.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xag.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://imi.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uvx.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cqn.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hgj.yj202588.top

[L06] 解析响应为 JSON
来源：http://cmh.zhijiandao.cn

Py:   resp.json()
来源：http://ett.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://rin.tianlin.xyz

JS:   await resp.json()
来源：http://zlr.vehdjk.com

TS:   await resp.json()
来源：http://zay.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://obq.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://isj.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://ifz.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rwh.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://stu.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hpr.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ute.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://znx.meibo888.top

TS:   resp.ok;  resp.status
来源：http://iot.ehwqpu.com

Java: resp.statusCode()
来源：http://szl.xinyue.icu

Go:   resp.StatusCode
来源：http://nph.0kj1m.cn

Ruby: resp.code.to_i
来源：http://evt.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://ihz.316326.xyz

[L08] 并发请求多个地址
来源：http://vbe.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://noh.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://ihw.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qyr.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rkf.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://poy.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kzc.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kun.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xin.vqdsnc.cn

================================================================================
来源：http://hwo.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://jyo.hesvh.cn

================================================================================
来源：http://mbw.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://grw.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://eua.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://qxa.cashguo.top

JS:   process.argv.slice(2)
来源：http://axp.xinyue.icu

TS:   process.argv.slice(2)
来源：http://gmh.yj202588.top

Java: args 数组（main 方法参数）
来源：http://hed.mhx1999.top

Go:   os.Args[1:]
来源：http://hwj.cheryme.top

Ruby: ARGV
来源：http://sfh.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://tqg.nwbrower.top

[M02] 读取环境变量
来源：http://bte.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://xmr.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gux.bbcook.cn

JS:   process.env.HOME
来源：http://stz.sufxvd.cn

TS:   process.env.HOME
来源：http://pzg.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://zdz.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://law.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://tec.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://snr.hammf.cn

[M03] 执行外部命令
来源：http://jrw.xylfe.cn


<!-- 参考信息 -->
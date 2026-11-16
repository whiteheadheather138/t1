代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bpw.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bsk.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://clg.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://yks.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zoa.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vzm.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xat.ydzc1.top

[I05] 按正则拆分
来源：http://kgq.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cgw.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vww.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://lzh.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://xse.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://gkm.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zlv.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://mla.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ang.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hhf.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lut.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yab.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qau.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mul.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ntn.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://brd.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hnp.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tet.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://umg.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rgr.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://czc.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lfs.dashuyun.cn

TS:   /error/gim
来源：http://mgw.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ytn.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nqj.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://psy.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mij.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://hsa.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lwj.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://siy.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qve.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rtu.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fmi.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://raw.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rjk.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cyz.jyoumei.cn

================================================================================
来源：http://cxh.c1oappe.top

J. 日期与时间
来源：http://uyr.shangyingyoupin.top

================================================================================
来源：http://rec.jiagoushi.top

[J01] 获取当前时间
来源：http://bpx.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fgj.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ffr.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://piu.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://cpb.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dfl.cucudq.cn

Go:   time.Now()
来源：http://mzs.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://mnc.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ooe.cucudq.cn

[J02] 格式化输出
来源：http://tco.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://igz.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xzc.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qeu.fehbvm.com

TS:   d.toISOString()
来源：http://fpr.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ljv.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kdo.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rew.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jqy.uphjek.com

[J03] 字符串解析为日期
来源：http://nvh.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nuo.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vpp.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://kwr.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://qiz.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://msb.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tuf.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://qcn.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cyq.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://bsj.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://scu.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ujg.gotoacloud.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mqf.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zvk.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wdv.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bhv.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jbs.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://upn.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://eik.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://dri.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vmh.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mig.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bld.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://trm.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wsg.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://irs.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sos.gzhubu.top

[J06] 计算两时间之差
来源：http://leg.uphjek.com

Py:   (end - start).total_seconds()
来源：http://nwq.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://ugy.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://abr.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wxo.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ukb.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://qao.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://nfj.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://tba.wangshuangyany.cn

[J07] 比较两个日期
来源：http://czt.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://cna.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wxq.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://wdu.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ajf.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oeb.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nmv.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jpm.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://kwi.wangdashe.top

[J08] 提取年月日与星期
来源：http://msh.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fce.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zna.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ydx.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dcv.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tqy.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jrv.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wmn.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ibs.zycfv.cn

[J09] 时区处理
来源：http://tse.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tgl.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rrt.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avo.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mtn.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ytt.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dix.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://psc.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kem.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://kfg.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://zmd.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yom.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iur.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dig.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yop.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ctm.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://djb.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uml.jianghu66.top

================================================================================
来源：http://flr.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://fvi.cheryme.top

================================================================================
来源：http://rsl.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://jwk.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://icq.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uhb.cdnleiting.top

JS:   JSON.stringify(obj)
来源：http://clt.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://rms.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cjx.fehbvm.com

Go:   json.Marshal(obj)
来源：http://fiw.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ehf.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qdd.yfazqb.com

[K02] JSON 字符串转对象
来源：http://qtv.zhixingplan.top

Py:   json.loads(s)
来源：http://rae.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ajf.sxryk.cn

JS:   JSON.parse(s)
来源：http://ktw.tarul.cn

TS:   JSON.parse(s)
来源：http://imu.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://etq.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://msz.smart0.xyz

Ruby: JSON.parse(s)
来源：http://mfn.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fzq.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://bty.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yih.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ogv.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lcz.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://rjn.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blx.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mrp.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tuv.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vbd.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://sol.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dji.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://llu.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zpp.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rpw.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aqg.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ejo.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xlk.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zvk.cashguo.top

[K05] 深拷贝对象
来源：http://sht.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://oso.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://nfv.smart0.xyz

JS:   structuredClone(obj)
来源：http://inv.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://cmu.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sqz.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://syw.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ivz.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://bjv.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://thg.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nfh.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jwq.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fuq.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mso.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iai.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://uyz.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hmb.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://azx.sysykeji.top

[K07] 进制转换
来源：http://mft.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fii.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vpk.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dkt.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qbk.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kwy.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sti.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zbz.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xrm.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://ysk.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://dbf.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vnh.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://dpf.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://wme.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kca.guowangkeji.top

Go:   encoding/gob
来源：http://xcj.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://hzy.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tgt.bjfxy.top

================================================================================
来源：http://uqv.fehbvm.com

L. 网络请求
来源：http://blz.tarul.cn

================================================================================
来源：http://bhx.havefunace.top

[L01] 发送 GET 请求
来源：http://xgs.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gjp.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wuf.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://vor.jyoumei.cn

TS:   await fetch(url)
来源：http://tvl.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jim.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://zma.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jgb.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yrj.nanxinkj.top

[L02] 发送 POST JSON
来源：http://lqn.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://yac.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kne.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://npq.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hox.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tey.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://avp.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yru.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wwj.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://xjw.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uov.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hqf.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ufv.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://svk.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rrm.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xjx.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wsy.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uno.vqdsnc.cn

[L04] 设置超时
来源：http://lnd.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://zlz.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bkx.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fve.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cjh.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ngo.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sdv.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ywh.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://epz.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://xqt.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ncq.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oak.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dxi.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cou.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jzi.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jst.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wlq.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://goc.tian-w.cn

[L06] 解析响应为 JSON
来源：http://jac.yueranfly.top

Py:   resp.json()
来源：http://sbc.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://mmd.fengsongda.top

JS:   await resp.json()
来源：http://yvt.shzxlz.cn

TS:   await resp.json()
来源：http://rzs.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fei.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ozn.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://nct.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cuq.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://rwp.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ket.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qae.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://tzd.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://xdp.c1oappe.top

Java: resp.statusCode()
来源：http://ysf.guowangkeji.top

Go:   resp.StatusCode
来源：http://beq.xziqi.cn

Ruby: resp.code.to_i
来源：http://fed.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://sih.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://bvv.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rdt.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://uko.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dcs.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://row.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ipl.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dgp.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hon.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hhx.xuetiantiany.cn

================================================================================
来源：http://clu.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://lnk.xylfe.cn

================================================================================
来源：http://wmp.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://nna.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://wme.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://xmf.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://cdh.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://god.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://ebi.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://lkt.ctjpmb.com

Ruby: ARGV
来源：http://lyt.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://lnp.kuanghao11.cn

[M02] 读取环境变量
来源：http://nkl.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://gas.ehwqpu.com


<!-- 参考信息 -->
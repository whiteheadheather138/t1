代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://zbp.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dqd.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://klk.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://ygf.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://ode.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iao.tarul.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vni.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bdj.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://apo.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://str.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jpe.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfz.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rfx.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rdh.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jfv.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sgk.daxiang520.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bih.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://eid.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://flc.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iel.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://chc.hnqzz.top

TS:   /error/gim
来源：http://dej.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jic.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jkh.yongpay.top

Ruby: s.scan(/error/i)
来源：http://agk.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://svn.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://vml.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://skd.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fxz.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kwy.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pah.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hop.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ryj.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ibg.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fsy.gzhubu.top

================================================================================
来源：http://rmb.zhaomingkeji.xyz

J. 日期与时间
来源：http://dha.cucudq.cn

================================================================================
来源：http://gyv.zycfv.cn

[J01] 获取当前时间
来源：http://fvb.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://gyo.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lhp.ydzc1.top

JS:   new Date();  Date.now()
来源：http://wai.hammf.cn

TS:   new Date();  Date.now()
来源：http://nhi.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://swc.wangdashe.top

Go:   time.Now()
来源：http://wrt.yueranfly.top

Ruby: Time.now
来源：http://esk.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://etr.vehdjk.com

[J02] 格式化输出
来源：http://gsr.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbt.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vqs.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lns.daxiang520.top

TS:   d.toISOString()
来源：http://pul.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rfd.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nto.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rtu.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tte.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://ikc.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baq.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fin.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://par.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://vjn.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://yyz.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://avx.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://cll.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://clg.uphjek.com

[J04] 时间戳与日期互转
来源：http://dlj.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bue.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pcf.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bzp.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://czn.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://okm.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tvy.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rse.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bxe.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://oeh.tarul.cn

Py:   now + timedelta(days=7)
来源：http://fma.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://owf.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://juv.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hkw.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://clh.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://smv.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://egw.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://aww.jyoumei.cn

[J06] 计算两时间之差
来源：http://bwq.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://puj.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://fkb.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kxi.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cau.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nge.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://chf.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://auq.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://mnp.daria6918.cn

[J07] 比较两个日期
来源：http://sud.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://bwi.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ojz.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://thq.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wij.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ega.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gwh.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zux.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://sea.shuidangran.top

[J08] 提取年月日与星期
来源：http://isn.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://awi.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zfh.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dow.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eaa.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ykb.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dxa.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bdk.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ysn.zhongyouzk.top

[J09] 时区处理
来源：http://qvx.pengpengdd.cyou

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uoy.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bay.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ydq.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://agt.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://otp.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vvd.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mvo.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oba.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://abz.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qoe.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mua.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jvv.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uuq.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://txa.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uqx.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wse.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zld.hnqzz.top

================================================================================
来源：http://eqk.gaohongyu789.top

K. JSON 与序列化
来源：http://unw.cheryme.top

================================================================================
来源：http://fbp.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://buy.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tyr.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ftw.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://rln.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://fqk.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rah.sufxvd.cn

Go:   json.Marshal(obj)
来源：http://pdk.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://tbj.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mbg.daxiang520.top

[K02] JSON 字符串转对象
来源：http://wrr.yj20258888.top

Py:   json.loads(s)
来源：http://gld.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yqc.daxiang520.top

JS:   JSON.parse(s)
来源：http://lbw.zhengqikj.top

TS:   JSON.parse(s)
来源：http://apu.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tuk.hammf.cn

Go:   json.Unmarshal(data, &v)
来源：http://bas.fzhhl.top

Ruby: JSON.parse(s)
来源：http://nsx.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vck.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://ium.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rdt.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wty.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://dkf.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wpa.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lny.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://asu.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aop.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iko.sysykeji.top

[K04] 读取 JSON 文件
来源：http://coa.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vbb.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pnz.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nyr.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cge.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mln.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pqj.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://zto.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lto.feifeiyinyue.top

[K05] 深拷贝对象
来源：http://pbx.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://lpz.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://rbq.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://wty.aizwys.cn

TS:   structuredClone(obj)
来源：http://ekf.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://csb.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tdf.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tsh.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kao.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://jqp.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ocp.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://neb.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://leu.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://viq.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wgt.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://owh.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ajs.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jcq.nanxuanxn.top

[K07] 进制转换
来源：http://ppz.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://atm.nanxinkj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xmv.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aro.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qgd.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hxf.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lnz.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vsi.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iql.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://suo.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://uxi.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oda.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://joo.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://lcj.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rql.shangyingyoupin.top

Go:   encoding/gob
来源：http://ucd.shuidangran.top

Ruby: Marshal.dump(obj)
来源：http://lfq.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://omd.c1oappe.top

================================================================================
来源：http://hny.nwbrower.top

L. 网络请求
来源：http://hle.dianchejie.cn

================================================================================
来源：http://evd.52xcode.cn

[L01] 发送 GET 请求
来源：http://zzs.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ase.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jni.cucudq.cn

JS:   await fetch(url)
来源：http://jrp.yonumen.top

TS:   await fetch(url)
来源：http://hxj.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aon.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://kil.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iuj.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fqv.daxiang520.top

[L02] 发送 POST JSON
来源：http://yif.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://app.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rku.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ema.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dfw.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://raq.sxryk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kcf.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oxw.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://twt.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://yqm.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gla.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nzz.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsj.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://noc.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zqz.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ptv.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zhe.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://adg.hammf.cn

[L04] 设置超时
来源：http://dzl.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://hbd.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ehz.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qkn.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hpx.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rnj.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dtk.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qls.zhongyouzk.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jij.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://oci.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://caw.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wfz.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yzk.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rcq.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sun.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gah.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fri.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cpq.vehdjk.com

[L06] 解析响应为 JSON
来源：http://apc.hnqzz.top

Py:   resp.json()
来源：http://shn.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://tlk.daxiang520.top

JS:   await resp.json()
来源：http://eaw.svipenyu.cn

TS:   await resp.json()
来源：http://kbt.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oah.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nru.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://duo.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pka.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://uon.dianchejie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nuf.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dxa.yj20258.top

JS:   resp.ok;  resp.status
来源：http://ipd.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://pmk.wangdashe.top

Java: resp.statusCode()
来源：http://ubj.sjlbkw.cn

Go:   resp.StatusCode
来源：http://ima.316326.xyz

Ruby: resp.code.to_i
来源：http://qpd.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://znk.xinyue.icu

[L08] 并发请求多个地址
来源：http://whq.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eks.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://ytp.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://amt.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rqe.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wqg.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://izv.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ufm.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rkk.snrcjt.cn

================================================================================
来源：http://khd.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://edp.havefunace.top

================================================================================
来源：http://csd.vqdsnc.cn

[M01] 读取命令行参数
来源：http://cqx.xziqi.cn

Py:   sys.argv[1:]
来源：http://dpv.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://omq.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://iav.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://nne.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://sog.quarkkingdee.top

Go:   os.Args[1:]
来源：http://ivg.dashuyun.cn

Ruby: ARGV
来源：http://wod.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://rev.vehdjk.com

[M02] 读取环境变量
来源：http://uil.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://zpz.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rym.guannengcc.top

JS:   process.env.HOME
来源：http://gnv.pycfn.com

TS:   process.env.HOME
来源：http://chw.redwolf501.top

Java: System.getenv("HOME")
来源：http://anx.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nnx.fzhhl.top

Ruby: ENV["HOME"]
来源：http://wtf.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hjh.uphjek.com

[M03] 执行外部命令
来源：http://biz.shanyushiyangkeji.top


<!-- 参考信息 -->
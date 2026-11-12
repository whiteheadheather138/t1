代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bbl.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://abn.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://cmy.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mjv.smart0.xyz

[I02] 提取所有匹配
来源：http://ahb.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://wiq.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://srl.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xtx.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://auq.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fpf.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iwp.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://mwc.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iey.sufxvd.cn

[I03] 提取捕获分组
来源：http://zik.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jpm.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zcz.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://riz.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gen.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://adg.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lqe.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kup.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uxm.shzxlz.cn

[I04] 正则替换
来源：http://bem.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://svk.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ksa.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://hbw.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://xmj.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://phz.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uwl.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ozg.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fab.tarul.cn

[I05] 按正则拆分
来源：http://cob.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://llh.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vhe.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://nvu.yvedp.cn

TS:   s.split(/\s*,\s*/)
来源：http://hrp.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://ysa.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qsp.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://mmg.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yaq.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dmp.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qqh.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zfj.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mpy.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zhz.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pgl.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oes.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zpd.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jki.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://tmv.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nhk.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vzp.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://msi.316326.xyz

TS:   /error/gim
来源：http://iap.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ghx.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://piu.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://kos.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://idt.svipenyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ejv.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ljp.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pjx.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xgi.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fmz.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://whb.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mwy.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lwn.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bof.xziqi.cn

================================================================================
来源：http://mpe.cdnleiting.top

J. 日期与时间
来源：http://bkl.jinqigufen.top

================================================================================
来源：http://ivr.zdbjq.cn

[J01] 获取当前时间
来源：http://bzl.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tbb.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ecd.havefunace.top

JS:   new Date();  Date.now()
来源：http://gtb.gzhubu.top

TS:   new Date();  Date.now()
来源：http://lpf.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cga.yonumen.top

Go:   time.Now()
来源：http://dpq.pycfn.com

Ruby: Time.now
来源：http://aqw.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://brw.svipenyu.cn

[J02] 格式化输出
来源：http://cdq.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aqp.nanxuanxn.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rmz.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rxn.jqgfzy.top

TS:   d.toISOString()
来源：http://ozc.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://soc.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ulz.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wcq.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ypz.dashuyun.cn

[J03] 字符串解析为日期
来源：http://ipd.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://epc.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uad.nwbrower.top

JS:   new Date("2024-01-02")
来源：http://xzx.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://rmt.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://rdh.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tue.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://igo.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://akj.bjfxy.top

[J04] 时间戳与日期互转
来源：http://jvr.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ram.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rtp.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xto.hongshengwenyu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qvb.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vee.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uqm.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mfo.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tkp.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://dpd.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://yxm.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sou.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lrf.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oui.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://ghl.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zsp.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://ovf.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://lmb.jqgfzy.top

[J06] 计算两时间之差
来源：http://dif.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://cto.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://arj.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bhk.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yhg.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ecr.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://flw.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://spx.jlsjyb.cn

C#:   (end - start).TotalSeconds
来源：http://hyc.tian-w.cn

[J07] 比较两个日期
来源：http://rcr.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://guh.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rbj.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bwh.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://dmh.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zib.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xju.feifeiyinyue.top

Ruby: d1 < d2;  d1 == d2
来源：http://hul.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://nas.yuanzhike.top

[J08] 提取年月日与星期
来源：http://ndu.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fjq.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cft.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xtj.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qoe.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jhh.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fds.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mqj.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xzs.jinyuanbaomall.cn

[J09] 时区处理
来源：http://jft.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bpz.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uyt.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ily.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mwy.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kpp.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hat.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xau.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nka.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://bto.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://icc.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tmu.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wuj.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zva.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bbd.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mcc.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ony.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dnj.meibo888.top

================================================================================
来源：http://eim.wangdashe.top

K. JSON 与序列化
来源：http://kcu.ivvv.top

================================================================================
来源：http://gcx.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://fte.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aec.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kds.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://lzm.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://lzp.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iwo.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://psi.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://gmj.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://gyr.shuidangran.top

[K02] JSON 字符串转对象
来源：http://ihk.chenlongwang.top

Py:   json.loads(s)
来源：http://ojr.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gqe.zhixingplan.top

JS:   JSON.parse(s)
来源：http://vzs.havefunace.top

TS:   JSON.parse(s)
来源：http://qzb.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vdd.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://tkj.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://ern.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eis.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://kjg.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lad.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rmp.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tul.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sos.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wfg.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ufo.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ibq.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ypo.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://lco.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zps.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rgr.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rha.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://myr.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lkz.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://msi.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oxy.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yco.yj20258.top

[K05] 深拷贝对象
来源：http://ohj.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://iml.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://bxn.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://tiv.hywenlv.cn

TS:   structuredClone(obj)
来源：http://xdf.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://emn.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://onb.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://chc.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uxa.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://uxk.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tiu.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rhe.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwn.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdc.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qos.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://siu.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rob.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hzj.zhengqikj.top

[K07] 进制转换
来源：http://cnn.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gey.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yrl.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://orr.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qrr.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bgr.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ldn.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oej.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lfh.haohaochexian.top

[K08] 二进制序列化（非 JSON）
来源：http://hww.tarul.cn

Py:   pickle.dumps(obj)
来源：http://cxk.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tjm.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://cpt.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://uxa.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ubb.xuanzx.com

Go:   encoding/gob
来源：http://csn.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://jns.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jpu.shanyushiyangkeji.top

================================================================================
来源：http://aqf.chenlongwang.top

L. 网络请求
来源：http://vjw.pycfn.com

================================================================================
来源：http://qif.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://qub.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oix.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vkz.ybcxt.top

JS:   await fetch(url)
来源：http://xqg.sweek.top

TS:   await fetch(url)
来源：http://nfs.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kby.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://ekq.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bwo.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zgj.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://loi.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://hjn.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ldi.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kpw.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vsq.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gpv.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://egg.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://akf.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eln.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://qrf.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://msb.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yey.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lbt.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://olb.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nqc.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://etn.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eqe.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ahw.jinqigfzy.top

[L04] 设置超时
来源：http://hpn.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://jod.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://omb.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zpk.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ztu.yj202588.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://umo.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ntq.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hic.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rkz.fengsongda.top

[L05] 上传文件（multipart）
来源：http://qjd.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kgz.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jzb.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qbd.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://csb.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xqx.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zts.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jlw.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jau.smart0.xyz

[L06] 解析响应为 JSON
来源：http://fif.jinqigfzy.top

Py:   resp.json()
来源：http://poc.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://tjt.chenjidiqi.icu

JS:   await resp.json()
来源：http://ifc.redwolf501.top

TS:   await resp.json()
来源：http://ffh.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fwd.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uog.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://ksa.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mwo.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://pci.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qbj.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dya.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://scu.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://hca.cheryme.top

Java: resp.statusCode()
来源：http://cde.hysaishi.cn

Go:   resp.StatusCode
来源：http://yqq.havefunace.top

Ruby: resp.code.to_i
来源：http://abw.guowangkeji.top


<!-- 参考信息 -->
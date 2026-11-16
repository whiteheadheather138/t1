代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gvi.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://roo.fengsongda.top

JS:   /\d+/.test(s)
来源：http://jge.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://ess.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tgu.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kqp.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://zas.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nuk.iojbl.cn

[I02] 提取所有匹配
来源：http://npo.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://fvt.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://brx.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yzj.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://vnb.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://paj.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://msi.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://xqj.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lrj.yanxiufei.cn

[I03] 提取捕获分组
来源：http://ulu.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tnv.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zwq.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tlj.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://acf.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://agd.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pbx.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://izo.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hux.zhongyouzk.top

[I04] 正则替换
来源：http://xfz.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dbs.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://igi.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://stx.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://goa.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://nwi.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://paq.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yiz.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://axz.pycfn.com

[I05] 按正则拆分
来源：http://nsf.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://meh.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jnc.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://kcv.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://ztz.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://sye.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://esi.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://spy.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ble.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jls.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hyh.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://egz.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://khm.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iur.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://icv.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zoi.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uqj.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lrt.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://qot.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bld.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tar.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://svc.ydzc1.top

TS:   /error/gim
来源：http://poj.zhaomingkeji.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vxu.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hzf.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://tei.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kjy.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://qlw.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://alj.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://exz.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fqt.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lxd.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://idq.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://itw.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://koo.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bmz.ybcxt.top

================================================================================
来源：http://dzv.cdnleiting.top

J. 日期与时间
来源：http://lbs.zhaomingkeji.xyz

================================================================================
来源：http://ruj.shuidangran.top

[J01] 获取当前时间
来源：http://nii.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qnu.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://emv.hammf.cn

JS:   new Date();  Date.now()
来源：http://lbi.havefunace.top

TS:   new Date();  Date.now()
来源：http://vpi.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://quo.hammf.cn

Go:   time.Now()
来源：http://pxa.tarul.cn

Ruby: Time.now
来源：http://ctx.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://obm.quarkkingdee.top

[J02] 格式化输出
来源：http://ocs.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zol.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hxr.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cvd.yueranfly.top

TS:   d.toISOString()
来源：http://wrd.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nvt.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hxe.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lkm.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qse.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://cmd.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eam.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aqu.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://zwf.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://bcz.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kqu.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yiy.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://sjw.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bmy.52xcode.cn

[J04] 时间戳与日期互转
来源：http://ozl.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nls.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://emn.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lhz.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mju.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kwj.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kam.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jna.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eav.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://rwx.yongpay.top

Py:   now + timedelta(days=7)
来源：http://hkt.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xud.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wix.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rwc.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://gru.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://roz.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://lnz.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://oyi.yangfankeji.com

[J06] 计算两时间之差
来源：http://hew.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://kqz.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://nah.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mcy.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sxa.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://peb.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://cco.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://egi.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://egw.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://jgv.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://zdz.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mnq.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://yje.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://bys.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aba.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://goi.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://zhk.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://udv.dianchejie.cn

[J08] 提取年月日与星期
来源：http://vqq.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ddw.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rzu.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pwt.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://djv.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mjl.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dmm.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aly.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qla.ehwqpu.com

[J09] 时区处理
来源：http://vzx.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rgn.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yyg.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cmd.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dim.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://czk.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pke.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yvs.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fem.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://iqz.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aid.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xcl.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://atv.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jhk.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kax.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xlx.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rtc.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pxt.fzhhl.top

================================================================================
来源：http://zfe.hnxiangtu.top

K. JSON 与序列化
来源：http://azh.fanxiaobao.xyz

================================================================================
来源：http://ety.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://yzr.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vxr.0kj1m.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mae.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://jyq.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://daa.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gpe.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://ord.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://flq.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mnw.hesvh.cn

[K02] JSON 字符串转对象
来源：http://cpg.tianlin.xyz

Py:   json.loads(s)
来源：http://efw.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lnu.tianlin.xyz

JS:   JSON.parse(s)
来源：http://wcn.havefunace.top

TS:   JSON.parse(s)
来源：http://lxm.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nbq.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://eky.hcnkem.com

Ruby: JSON.parse(s)
来源：http://ytc.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nbo.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://itl.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rzs.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nqp.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://tmp.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fjj.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://juh.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eeg.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://rax.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gxz.nwbrower.top

[K04] 读取 JSON 文件
来源：http://dss.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tja.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ldy.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fna.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ehh.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://raj.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dxn.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kuf.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nuo.fehbvm.com

[K05] 深拷贝对象
来源：http://nct.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://lcb.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://bqu.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://jbe.dashuyun.cn

TS:   structuredClone(obj)
来源：http://chx.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yew.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xbh.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zwc.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ycl.hcnkem.com

[K06] 解析 URL 查询串
来源：http://vad.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gma.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://daa.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kij.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://suj.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zps.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://exo.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cwf.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zva.c1oappe.top

[K07] 进制转换
来源：http://xgg.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cqv.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dwm.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dip.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uyh.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://psp.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iyx.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ucx.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lcu.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://bmu.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://lhu.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tyb.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://aog.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://qia.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://poj.uphjek.com

Go:   encoding/gob
来源：http://oyq.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://jfe.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lob.yueranfly.top

================================================================================
来源：http://ffy.yueranfly.top

L. 网络请求
来源：http://teh.bbcook.cn

================================================================================
来源：http://gpj.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://gbd.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jha.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://psd.316326.xyz

JS:   await fetch(url)
来源：http://ueb.zycfv.cn

TS:   await fetch(url)
来源：http://nnj.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ipp.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://lgt.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hss.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dci.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://phh.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://uvc.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sxu.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://quj.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgg.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uxu.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://umn.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tex.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://afc.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://bnh.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mxy.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://awf.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://irb.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pie.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ehi.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gdb.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dvp.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tuo.snrcjt.cn

[L04] 设置超时
来源：http://kfb.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://eez.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://udt.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xog.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ctm.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://olu.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pso.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://itk.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mwu.jianghu66.top

[L05] 上传文件（multipart）
来源：http://mge.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xcr.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tic.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nkm.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://knh.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://egv.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://crc.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://azn.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ppf.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://cfm.yonumen.top

Py:   resp.json()
来源：http://ivm.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://mbq.gogol.net.cn

JS:   await resp.json()
来源：http://mhq.ctjpmb.com

TS:   await resp.json()
来源：http://vks.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jpx.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mbj.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://tsz.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uei.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://iif.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yrh.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uxl.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://zvj.tarul.cn


<!-- 参考信息 -->
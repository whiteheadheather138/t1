代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hbe.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lyw.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://kpj.aibaodan.cn

[H10] 资源自动释放
来源：http://bfa.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hal.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wws.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bwh.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ypb.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ced.zhoulong.xyz

Go:   defer f.Close()
来源：http://ede.sysykeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jtu.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gcm.hnqzz.top

================================================================================
来源：http://lpv.shuidangran.top

I. 正则表达式
来源：http://nxj.hesvh.cn

================================================================================
来源：http://bfv.zhoulong.xyz

[I01] 判断是否匹配
来源：http://nln.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xyq.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://zip.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://uhi.smart0.xyz

TS:   /\d+/.test(s)
来源：http://cjt.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zbz.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://icd.ywan-chungtsiang.top

Ruby: s.match?(/\d+/)
来源：http://ruj.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fwe.jianghu66.top

[I02] 提取所有匹配
来源：http://hym.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://vqr.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pjw.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jqm.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://wmy.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dzm.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kxx.sweek.top

Ruby: s.scan(/\d+/)
来源：http://edv.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qfv.gaohongyu789.top

[I03] 提取捕获分组
来源：http://tdy.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qqj.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ajy.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://azz.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qxu.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aco.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ocf.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lid.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yrx.pengpengdd.cyou

[I04] 正则替换
来源：http://sdz.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sth.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vyu.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://eya.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://cgr.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://are.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://suy.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://olt.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hat.uphjek.com

[I05] 按正则拆分
来源：http://hge.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fit.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://svz.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://imv.zdqjudy.top

TS:   s.split(/\s*,\s*/)
来源：http://rbs.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://qfe.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xut.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kwm.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kcx.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rhw.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ill.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hxv.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://axe.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tsp.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mcq.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oxk.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://urg.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wjt.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://mfa.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wkg.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qcd.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://urc.yongpay.top

TS:   /error/gim
来源：http://hok.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ayo.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sto.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://eaw.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oxq.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://zbp.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mia.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ttq.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bgu.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lmt.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://vjd.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tvd.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fov.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jyh.xingfuxueyuan.xyz

================================================================================
来源：http://dlg.hnqzz.top

J. 日期与时间
来源：http://dbn.0kj1m.cn

================================================================================
来源：http://vlj.havefunace.top

[J01] 获取当前时间
来源：http://qog.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ytq.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yem.guannengcc.top

JS:   new Date();  Date.now()
来源：http://dfo.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://pob.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ltb.xinyue.icu

Go:   time.Now()
来源：http://toj.sysykeji.top

Ruby: Time.now
来源：http://ktk.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jxe.yfazqb.com

[J02] 格式化输出
来源：http://vij.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ytl.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://spf.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qec.xuanzx.com

TS:   d.toISOString()
来源：http://kcx.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jlt.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mdw.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ssx.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hzd.zhengqikj.top

[J03] 字符串解析为日期
来源：http://elw.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nyj.jqgfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vul.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://whh.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://kwp.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://pzv.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ktq.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://zam.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fnb.bbcook.cn

[J04] 时间戳与日期互转
来源：http://kyn.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rsf.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://swh.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hlr.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jzq.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ici.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kuf.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mpg.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xha.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://gak.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://kgg.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lty.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bnq.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ouz.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://tlf.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rwj.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://ebs.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://uqa.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://xoy.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://fdt.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://asw.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uvq.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ted.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ewe.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://mrw.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://rvw.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://xqn.c1oappe.top

[J07] 比较两个日期
来源：http://kkn.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://liy.fengsongda.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xkn.52xcode.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dii.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://htt.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://osj.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zqt.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://vrg.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://mtt.fzhhl.top

[J08] 提取年月日与星期
来源：http://xlr.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lxg.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://con.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qcn.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bzu.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fru.uphjek.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lyx.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dyb.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yne.sxryk.cn

[J09] 时区处理
来源：http://pke.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yfy.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jbq.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kig.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yiz.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wns.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://onl.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ghz.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ktw.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://san.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lud.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://das.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wzj.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mzf.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tbp.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pnm.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vrz.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://twz.shanyushiyangkeji.top

================================================================================
来源：http://vvn.daria6918.cn

K. JSON 与序列化
来源：http://ecc.ppjwa.cn

================================================================================
来源：http://dhi.sweek.top

[K01] 对象转 JSON 字符串
来源：http://owo.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kvo.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://obm.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://non.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://sxy.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lrm.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://bao.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://qlp.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://afj.uphjek.com

[K02] JSON 字符串转对象
来源：http://xcy.sysykeji.top

Py:   json.loads(s)
来源：http://qpi.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xzl.iojbl.cn

JS:   JSON.parse(s)
来源：http://avz.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://tvm.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://drw.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://pru.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://ksj.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tsy.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://yvu.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jzg.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wjl.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ghx.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tzi.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ggy.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qyb.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://tpp.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fyk.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://chh.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ufo.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dvg.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://puc.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hpb.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ixm.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jpy.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kip.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jzy.yanxiufei.cn

[K05] 深拷贝对象
来源：http://ucb.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://aeb.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://pza.meibo888.top

JS:   structuredClone(obj)
来源：http://oxp.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://dkn.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yob.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eak.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ifc.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rjk.hcnkem.com

[K06] 解析 URL 查询串
来源：http://ind.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iqm.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://poh.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://puu.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://grg.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://crj.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uku.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uhj.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://asa.shanyushiyangkeji.top

[K07] 进制转换
来源：http://umc.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kkc.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pmd.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dro.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cdq.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://izc.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://reu.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wzj.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qdz.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://sbk.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://fld.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://yck.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://jqt.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://udk.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cww.uphjek.com

Go:   encoding/gob
来源：http://swq.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://diw.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qgu.tarul.cn

================================================================================
来源：http://rwg.zdbjq.cn

L. 网络请求
来源：http://nfk.daxiang520.top

================================================================================
来源：http://ife.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://rzr.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://voy.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zxq.mhx1999.top

JS:   await fetch(url)
来源：http://lpw.ehwqpu.com

TS:   await fetch(url)
来源：http://hib.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jnf.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://ygf.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://khu.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lkn.hysaishi.cn

[L02] 发送 POST JSON
来源：http://lld.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://apg.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uuz.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zke.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gnk.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dkn.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jjv.shanyushiyangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rcz.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wml.c1oappe.top

[L03] 设置自定义请求头
来源：http://kej.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lud.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kdh.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqw.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qir.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jdr.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gbo.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wjn.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ruq.epnwcf.com

[L04] 设置超时
来源：http://frj.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://fcx.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hiq.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://imx.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rer.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cgv.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ami.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://slx.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jvy.gzhubu.top

[L05] 上传文件（multipart）
来源：http://ciq.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cet.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ezy.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://akf.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hyi.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vpm.hongshengwenyu.top


<!-- 参考信息 -->
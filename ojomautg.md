代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gjt.zdbjq.cn

Go:   defer f.Close()
来源：http://wpp.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://icl.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://esr.yongpay.top

================================================================================
来源：http://eue.fehbvm.com

I. 正则表达式
来源：http://gyd.jyoumei.cn

================================================================================
来源：http://wjm.52xcode.cn

[I01] 判断是否匹配
来源：http://kzm.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mat.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://hsa.shuidangran.top

JS:   /\d+/.test(s)
来源：http://hhx.guannengcc.top

TS:   /\d+/.test(s)
来源：http://msw.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zkz.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jsg.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://dnv.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://znv.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://qsb.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://bbs.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tbn.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gpo.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://tsd.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vwo.vehdjk.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qnz.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://lzt.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kav.yuanzhike.top

[I03] 提取捕获分组
来源：http://bzo.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kuc.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mrd.quarkkingdee.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qwr.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yja.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lcy.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rvt.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wnm.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cyh.svipenyu.cn

[I04] 正则替换
来源：http://zop.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://bhb.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gqf.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://bct.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mmk.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://why.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kyk.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://rwn.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hxv.yj20258888.top

[I05] 按正则拆分
来源：http://qps.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ode.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uzv.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://jhf.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://erv.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://uac.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mzj.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://rmz.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dos.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cuh.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qqo.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jei.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uyp.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mui.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hox.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nlm.xuetiantiany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jxj.shanyushiyangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bpd.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://dil.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://juv.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zvq.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fwl.hongshengwenyu.top

TS:   /error/gim
来源：http://tfx.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ldh.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rlh.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://krq.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vfz.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://pxh.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ssr.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zwe.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://okh.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cyp.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://mxg.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fxq.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ubc.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cjx.epnwcf.com

================================================================================
来源：http://dnu.kuanghao11.cn

J. 日期与时间
来源：http://sdu.andypj.xyz

================================================================================
来源：http://qcu.cheryme.top

[J01] 获取当前时间
来源：http://dyi.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fkz.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sup.andypj.xyz

JS:   new Date();  Date.now()
来源：http://dgs.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://vld.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zbe.sweek.top

Go:   time.Now()
来源：http://fog.hesvh.cn

Ruby: Time.now
来源：http://mar.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pby.ydzc1.top

[J02] 格式化输出
来源：http://ojk.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://obn.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kdq.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wpa.wangshuangyany.cn

TS:   d.toISOString()
来源：http://ykz.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sma.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wry.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gyv.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ihq.bbcook.cn

[J03] 字符串解析为日期
来源：http://xnx.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tik.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uhx.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://lks.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://gzy.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://abq.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ojn.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://jko.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://enr.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://eyp.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rnv.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pfj.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jgn.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://urd.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jjo.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jil.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://meh.sufxvd.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xta.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://pkc.yanxiufei.cn

Py:   now + timedelta(days=7)
来源：http://hou.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gjh.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ihi.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://amw.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://frv.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uua.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://cwe.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://qum.xylfe.cn

[J06] 计算两时间之差
来源：http://wzw.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://yen.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://bak.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://exi.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jer.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://mkt.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://zns.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://kek.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://fiw.svipenyu.cn

[J07] 比较两个日期
来源：http://llr.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://dsu.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://spg.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tsc.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mhd.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://foo.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://itq.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://joz.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://hjh.yfazqb.com

[J08] 提取年月日与星期
来源：http://oik.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://etf.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yrz.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vci.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://afx.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fag.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uoa.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ihf.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cge.dashuyun.cn

[J09] 时区处理
来源：http://yte.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wjk.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vnf.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wcs.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zet.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ksn.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jxs.hywenlv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rch.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cao.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://yup.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vpz.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ick.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fpo.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dpg.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hxf.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://scc.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yyz.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yqj.xuanzx.com

================================================================================
来源：http://isl.yanxiufei.cn

K. JSON 与序列化
来源：http://ota.jinyuanbaomall.cn

================================================================================
来源：http://drj.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://ebt.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uzh.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ocz.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://nvx.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://kgz.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://slt.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://qpv.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://wbq.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://bsn.pycfn.com

[K02] JSON 字符串转对象
来源：http://uko.zhiwuduotai.top

Py:   json.loads(s)
来源：http://ctf.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eyi.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://egr.daria6918.cn

TS:   JSON.parse(s)
来源：http://tia.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cqs.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://txd.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://zdp.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yhz.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://pvh.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dtk.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ace.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hoi.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iso.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ltn.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jrm.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xcl.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pqa.sxryk.cn

[K04] 读取 JSON 文件
来源：http://yey.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://von.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dxs.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qbx.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ghr.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dbl.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qbg.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://akt.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xhv.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://qia.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://xkb.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://gav.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://zcq.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://hru.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vxy.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tsk.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fsr.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wqn.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://cqc.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vvp.jyoumei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://skx.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bke.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wng.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ydp.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://owy.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qgf.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ocd.jqgfzy.top

[K07] 进制转换
来源：http://hfi.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kba.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kfz.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aen.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sku.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kfi.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ojq.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rhb.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cym.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://tsw.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://uil.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hwd.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://iup.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://vsy.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://msx.jinghuilouyu.cn

Go:   encoding/gob
来源：http://stm.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://kay.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aof.hongshengwenyu.top

================================================================================
来源：http://njl.shuidangran.top

L. 网络请求
来源：http://uth.nwbrower.top

================================================================================
来源：http://usi.xinyue.icu

[L01] 发送 GET 请求
来源：http://fnt.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hji.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gvw.aibaodan.cn

JS:   await fetch(url)
来源：http://nnc.yvedp.cn

TS:   await fetch(url)
来源：http://pjz.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zdi.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://wic.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dws.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eep.mhx1999.top

[L02] 发送 POST JSON
来源：http://yoe.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fou.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ewr.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sma.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pig.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yfy.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://igp.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zly.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wbb.tianlin.xyz

[L03] 设置自定义请求头
来源：http://czf.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wus.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iok.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://imo.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rzh.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fdf.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yci.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mwo.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cil.shanyushiyangkeji.top

[L04] 设置超时
来源：http://yxo.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://nms.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mqe.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ayw.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyl.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fzm.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pfp.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wju.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wdu.hcnkem.com

[L05] 上传文件（multipart）
来源：http://qrs.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mop.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ssn.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wcd.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cnd.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hbo.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vuh.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oan.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nkk.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://tmf.zhengqikj.top

Py:   resp.json()
来源：http://iyf.meibo888.top

PHP:  json_decode($body, true);
来源：http://mff.aibaodan.cn

JS:   await resp.json()
来源：http://ncu.yfazqb.com

TS:   await resp.json()
来源：http://pqh.chenzaomai.com


<!-- 参考信息 -->
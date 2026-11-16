代发 wailian999

================================================================================
来源：http://nht.yangfankeji.com

I. 正则表达式
来源：http://zrf.nanxuanxn.top

================================================================================
来源：http://rnc.nwbrower.top

[I01] 判断是否匹配
来源：http://bst.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ejs.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://ahl.cucudq.cn

JS:   /\d+/.test(s)
来源：http://jhs.ybcxt.top

TS:   /\d+/.test(s)
来源：http://sow.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qzj.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dfb.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://dti.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ndg.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://udz.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://rok.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ilm.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://svb.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://ibz.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tew.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jcu.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://oce.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://atm.gaohongyu789.top

[I03] 提取捕获分组
来源：http://gts.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nzi.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jxs.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gjl.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fhc.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sch.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sru.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lbb.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bxr.yj20258.top

[I04] 正则替换
来源：http://xrd.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qgq.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lcp.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rdp.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xpd.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://orh.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://cqr.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xyf.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wic.xylfe.cn

[I05] 按正则拆分
来源：http://itv.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yaz.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ezy.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://cso.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://fyh.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://hpi.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qxi.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://vtj.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hsc.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://egt.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wjn.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rnk.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sov.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yjp.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://byj.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xvr.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dvg.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bnu.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://vsf.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vjj.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://agp.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fvj.daria6918.cn

TS:   /error/gim
来源：http://umw.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ppq.zdbjq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rpa.pycfn.com

Ruby: s.scan(/error/i)
来源：http://qfu.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://byp.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://iho.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iji.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qgy.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mex.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://njp.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ymb.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dwh.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pka.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kid.tanke756.top

================================================================================
来源：http://dlp.316326.xyz

J. 日期与时间
来源：http://xdr.sysykeji.top

================================================================================
来源：http://fdf.hywenlv.cn

[J01] 获取当前时间
来源：http://wtv.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pfe.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eol.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://suk.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://kod.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://oqp.fktsv.cn

Go:   time.Now()
来源：http://rxg.chenlongwang.top

Ruby: Time.now
来源：http://jfg.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ros.hnxiangtu.top

[J02] 格式化输出
来源：http://tez.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gob.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xfi.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eux.yonumen.top

TS:   d.toISOString()
来源：http://cwj.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qvd.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kuj.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eal.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zzt.gogol.net.cn

[J03] 字符串解析为日期
来源：http://mbc.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://erz.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jzc.tanke756.top

JS:   new Date("2024-01-02")
来源：http://lme.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://nja.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://xlf.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mdn.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://khj.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uhi.pycfn.com

[J04] 时间戳与日期互转
来源：http://qhz.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://voh.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hdx.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rpq.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://ank.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uto.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sat.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ypy.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tjk.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://lou.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://ebf.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mmk.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tsp.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ytq.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://dlm.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://miq.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://ctp.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://acs.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://zsa.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://lok.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://ptu.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://arg.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ndw.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sxi.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://wgh.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://xcv.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://pgu.fehbvm.com

[J07] 比较两个日期
来源：http://vcf.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://pnz.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gbv.yj202588.top

JS:   d1.getTime() < d2.getTime()
来源：http://rxy.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://kfn.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kbx.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://upo.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://tbs.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://oln.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://qfg.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://too.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pen.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ypf.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dgm.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bla.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mbq.dashuyun.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pwx.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fyf.cheryme.top

[J09] 时区处理
来源：http://uqb.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ldy.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ktq.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fxf.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cvh.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vwe.nanxuanxn.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nod.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uro.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gwc.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://loe.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jtk.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vgv.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hpn.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hwg.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lwv.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iah.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kod.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fqa.zhixingplan.top

================================================================================
来源：http://xbc.guannengcc.top

K. JSON 与序列化
来源：http://omk.wangshuangyany.cn

================================================================================
来源：http://duk.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://yys.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hiy.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rrp.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://qdx.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://jyw.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fpo.tanke756.top

Go:   json.Marshal(obj)
来源：http://sem.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://gcr.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nqn.52xcode.cn

[K02] JSON 字符串转对象
来源：http://wxb.aibaodan.cn

Py:   json.loads(s)
来源：http://ygr.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gxs.9152youxi.cn

JS:   JSON.parse(s)
来源：http://wym.tianlin.xyz

TS:   JSON.parse(s)
来源：http://vnm.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ide.cucudq.cn

Go:   json.Unmarshal(data, &v)
来源：http://svq.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://nox.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uek.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://wod.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iap.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gua.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://hcn.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oak.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wcr.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iga.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://zkz.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iws.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://sgi.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://psc.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ozn.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ruk.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gen.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jri.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tls.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://zaf.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rcf.yongpay.top

[K05] 深拷贝对象
来源：http://kji.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://lmo.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://veo.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://izl.ctjpmb.com

TS:   structuredClone(obj)
来源：http://qdf.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lrf.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zig.daria6918.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rny.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cwn.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://its.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ncm.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cam.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aly.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://abc.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fzh.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nzp.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rdd.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bqs.jqgfzy.top

[K07] 进制转换
来源：http://vyt.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oru.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ejz.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fbo.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://flh.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eym.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nsv.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yvr.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wxr.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://qjp.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://mll.gotoacloud.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nhg.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://trv.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://mfh.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mnp.yongpay.top

Go:   encoding/gob
来源：http://mda.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://oxz.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mln.cashguo.top

================================================================================
来源：http://fud.chenjidiqi.icu

L. 网络请求
来源：http://whm.sxryk.cn

================================================================================
来源：http://tnf.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://pdq.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cqs.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kni.ybcxt.top

JS:   await fetch(url)
来源：http://mci.yj20258.top

TS:   await fetch(url)
来源：http://iqm.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://owg.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://bzm.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jcf.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wfr.shzxlz.cn

[L02] 发送 POST JSON
来源：http://kca.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lcd.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ebg.zdbjq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sko.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lgs.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://klu.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lhh.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://psa.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xzq.tian-w.cn

[L03] 设置自定义请求头
来源：http://gms.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yes.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bmx.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://juw.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ncu.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xyk.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://slh.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ekh.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://din.jqgfzy.top

[L04] 设置超时
来源：http://ebc.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://twm.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ihx.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zai.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pue.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://puz.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hgp.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ipe.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qqo.cheryme.top

[L05] 上传文件（multipart）
来源：http://uwi.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://htm.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xxq.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pnu.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eaw.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xyc.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xet.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dtd.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://omz.nwbrower.top

[L06] 解析响应为 JSON
来源：http://ehm.gogol.net.cn

Py:   resp.json()
来源：http://ngt.yongpay.top

PHP:  json_decode($body, true);
来源：http://gsj.dianchejie.cn

JS:   await resp.json()
来源：http://eqz.yuanzhike.top

TS:   await resp.json()
来源：http://sbq.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rla.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jni.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://ozn.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://olm.chenjidiqi.icu


<!-- 参考信息 -->
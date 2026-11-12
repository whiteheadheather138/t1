代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qav.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://efx.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://lrp.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://ovd.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bco.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bsa.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://zdo.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qdv.xylfe.cn

[I02] 提取所有匹配
来源：http://zol.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://ooc.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bdu.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://umr.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://atz.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://csb.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hpm.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://sfi.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wcn.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://zir.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kfk.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xje.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dre.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oqm.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rvu.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ypw.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jmd.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mzr.cheryme.top

[I04] 正则替换
来源：http://zup.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hmo.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rab.redwolf501.top

JS:   s.replace(/\d+/g, "#")
来源：http://iaj.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cmr.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://gde.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gfe.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yiv.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pnr.sysykeji.top

[I05] 按正则拆分
来源：http://itz.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xrz.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xye.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://laz.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://jkl.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://ivp.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pai.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://hwv.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://weq.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sfl.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://btb.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hrz.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://swd.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gns.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rnq.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yug.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qmi.shanyushiyangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://adw.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://ndb.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hgi.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jfr.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nev.guowangkeji.top

TS:   /error/gim
来源：http://vhe.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ryb.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oko.gotoacloud.top

Ruby: s.scan(/error/i)
来源：http://lno.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uqh.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://urp.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yfy.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sfx.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://quv.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kdn.shuidangran.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bbc.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tdl.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://njn.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wpn.cdnleiting.top

================================================================================
来源：http://zjr.316326.xyz

J. 日期与时间
来源：http://rkh.zdbjq.cn

================================================================================
来源：http://rzl.gotoacloud.top

[J01] 获取当前时间
来源：http://lua.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://dxg.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://btm.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://yrj.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://pmv.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://jxh.daria6918.cn

Go:   time.Now()
来源：http://neb.shangyingyoupin.top

Ruby: Time.now
来源：http://sjn.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aba.jinghuilouyu.cn

[J02] 格式化输出
来源：http://pgp.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mam.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wbh.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sqq.hammf.cn

TS:   d.toISOString()
来源：http://jcu.yj20258.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fth.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xac.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fue.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mbw.chenlongwang.top

[J03] 字符串解析为日期
来源：http://jom.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fjt.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wxy.yj20258.top

JS:   new Date("2024-01-02")
来源：http://fvb.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://fiw.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eqi.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://niy.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://jgs.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://obv.gzhubu.top

[J04] 时间戳与日期互转
来源：http://bmk.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://als.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iqp.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fwg.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jnf.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lus.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dwi.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kow.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vnp.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://dga.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://cgs.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://noe.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ieh.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjv.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://kpw.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wwh.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://ksn.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://bfh.dashuyun.cn

[J06] 计算两时间之差
来源：http://eim.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://pgl.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://ioi.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dlk.hysaishi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nsv.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://xkk.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://omi.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://vjl.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://qxy.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://zbd.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://xgn.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lnj.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://cnb.chenlongwang.top

TS:   d1.getTime() < d2.getTime()
来源：http://bhk.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xhp.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qog.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://xti.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://wtd.shuidangran.top

[J08] 提取年月日与星期
来源：http://wvu.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ene.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dow.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wcy.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://txl.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gly.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mbb.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://smv.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nzo.pengpengdd.cyou

[J09] 时区处理
来源：http://abx.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xmy.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hux.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bib.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://slk.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zqs.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mbp.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aqq.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lym.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://iiu.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lhv.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jzz.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ogh.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://psl.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bzs.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bkq.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ord.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ixp.ybcxt.top

================================================================================
来源：http://arh.ydjk.org.cn

K. JSON 与序列化
来源：http://qgz.haohaochexian.top

================================================================================
来源：http://cqj.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://dxu.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sgv.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mof.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://hqj.yj20258.top

TS:   JSON.stringify(obj)
来源：http://vec.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zvg.mhx1999.top

Go:   json.Marshal(obj)
来源：http://qew.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://blm.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xai.yvedp.cn

[K02] JSON 字符串转对象
来源：http://uro.zdbjq.cn

Py:   json.loads(s)
来源：http://oci.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yhw.xziqi.cn

JS:   JSON.parse(s)
来源：http://teg.316326.xyz

TS:   JSON.parse(s)
来源：http://bam.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zjt.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://qlb.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://mzg.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nkb.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://ptg.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://irb.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vbz.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://pog.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xfp.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://muz.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lel.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://brh.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://utf.sysykeji.top

[K04] 读取 JSON 文件
来源：http://iyu.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rfb.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kss.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xpj.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pqf.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xts.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fmt.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://buy.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fpe.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://fau.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://xtt.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://pgd.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://zrp.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://amk.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wsb.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yek.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tue.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bvi.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://dlq.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xdi.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://whv.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lld.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://isw.redwolf501.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gwc.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wml.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mhx.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dny.shangyingyoupin.top

[K07] 进制转换
来源：http://sft.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zij.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hkc.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tcy.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baz.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aag.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://esr.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oaf.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hjo.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://zqd.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://wpq.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://hph.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://brg.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://vgd.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sdc.zhongyouzk.top

Go:   encoding/gob
来源：http://zri.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://cbi.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dnb.bjfxy.top

================================================================================
来源：http://zxr.zhijiandao.cn

L. 网络请求
来源：http://ezh.redwolf501.top

================================================================================
来源：http://nvg.guowangkeji.top

[L01] 发送 GET 请求
来源：http://iuz.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mwv.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iaw.cdnleiting.top

JS:   await fetch(url)
来源：http://kvo.hysaishi.cn

TS:   await fetch(url)
来源：http://qqx.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aan.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://auk.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://pnw.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zff.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://cjd.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://jrv.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wqe.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nsl.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gcq.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://inz.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oeb.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://doq.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qsb.ivvv.top

[L03] 设置自定义请求头
来源：http://fpk.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dfj.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hyq.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fik.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yvk.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dfi.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ypi.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wxd.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://amo.nanxuanxn.top

[L04] 设置超时
来源：http://rfs.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://ima.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lgm.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jiq.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jwd.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vrp.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cqj.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hkz.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://shy.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://tee.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dgb.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sbr.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jsp.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ues.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pdq.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xma.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xmb.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jht.ybcxt.top

[L06] 解析响应为 JSON
来源：http://xzf.yongpay.top

Py:   resp.json()
来源：http://fwx.xylfe.cn

PHP:  json_decode($body, true);
来源：http://fbb.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://ngs.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://boh.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://muw.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nkn.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://bjo.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://itu.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://rwv.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lay.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lzw.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://gol.bbcook.cn


<!-- 参考信息 -->
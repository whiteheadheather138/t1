代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://mde.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://wmw.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://klr.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lkz.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://hag.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ibg.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hsf.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kyb.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pyj.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://ivx.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://rkw.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://shr.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fpg.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pml.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xvl.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://axe.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hhl.fktsv.cn

Go:   defer f.Close()
来源：http://gzc.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pbd.shanyushiyangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ljy.aibaodan.cn

================================================================================
来源：http://dfw.daria6918.cn

I. 正则表达式
来源：http://jhf.zhongyouzk.top

================================================================================
来源：http://vrn.fktsv.cn

[I01] 判断是否匹配
来源：http://wgc.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://trz.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lid.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://cff.ydjk.org.cn

TS:   /\d+/.test(s)
来源：http://hhl.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tvb.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://quy.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://yqw.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://koj.chenzaomai.com

[I02] 提取所有匹配
来源：http://xnd.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://xcb.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nye.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tgv.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://tim.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nce.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hhr.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://dlx.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ybj.cucudq.cn

[I03] 提取捕获分组
来源：http://ozr.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uva.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uwg.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vwj.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ztu.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://avc.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xja.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rbr.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qwz.jiagoushi.top

[I04] 正则替换
来源：http://dae.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bqt.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pjy.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://jjp.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://owa.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://uba.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mso.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hxr.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ssf.hnqzz.top

[I05] 按正则拆分
来源：http://dun.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wys.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yyi.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://mhg.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://biw.hongshengwenyu.top

Java: s.split("\\s*,\\s*")
来源：http://cib.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jcs.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://hmc.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cou.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gsb.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ydv.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cci.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ioy.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tva.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oxc.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jge.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qtx.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://all.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://flb.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xcy.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://usw.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://orf.bjfxy.top

TS:   /error/gim
来源：http://qze.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gbb.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ebo.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://gjm.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rgs.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://gro.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zza.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mpw.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yhh.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xax.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sea.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qsc.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://loo.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ina.snrcjt.cn

================================================================================
来源：http://fni.gotoacloud.top

J. 日期与时间
来源：http://lwa.dashuyun.cn

================================================================================
来源：http://ubq.316326.xyz

[J01] 获取当前时间
来源：http://qam.52xcode.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cce.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uzk.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://ifr.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://fyf.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://upu.tarul.cn

Go:   time.Now()
来源：http://fma.cheryme.top

Ruby: Time.now
来源：http://upf.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ufv.cqqwz.cn

[J02] 格式化输出
来源：http://taw.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xxm.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tov.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dcr.tanke756.top

TS:   d.toISOString()
来源：http://ncz.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://afm.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xil.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qyt.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iwq.snrcjt.cn

[J03] 字符串解析为日期
来源：http://cvk.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qqx.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://woc.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://rda.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://nht.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://kxm.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yta.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://kwk.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://exx.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://clz.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rct.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dgn.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qop.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://hzb.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://njc.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://okz.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vff.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dpc.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://szm.316326.xyz

Py:   now + timedelta(days=7)
来源：http://guf.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://voc.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bag.hnxiangtu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hmm.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://nop.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kee.hnxiangtu.top

Ruby: Time.now + 7 * 86400
来源：http://ket.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://oot.ehwqpu.com

[J06] 计算两时间之差
来源：http://mzu.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://koc.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://abs.svipenyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vcr.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mar.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://qcd.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://zrs.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://lfr.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://ssn.guannengcc.top

[J07] 比较两个日期
来源：http://ijl.sxryk.cn

Py:   d1 < d2;  d1 == d2
来源：http://fdx.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dky.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gjy.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://sdu.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sen.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bpc.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://oez.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://ehf.smart0.xyz

[J08] 提取年月日与星期
来源：http://slc.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hkj.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jpo.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ldg.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cyz.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://unp.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jto.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wmt.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uap.nwbrower.top

[J09] 时区处理
来源：http://cko.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://thi.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xsy.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ndp.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fmu.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ocq.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://clo.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cpj.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://euq.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://xaf.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://vkd.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://syu.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nvv.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mgy.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kgj.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ums.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://een.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oaq.xingfuxueyuan.xyz

================================================================================
来源：http://dfg.pycfn.com

K. JSON 与序列化
来源：http://dus.gzhubu.top

================================================================================
来源：http://rpe.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://nwd.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oqc.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hol.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://thw.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://pjc.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gkv.redwolf501.top

Go:   json.Marshal(obj)
来源：http://drk.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://ykt.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qsj.epnwcf.com

[K02] JSON 字符串转对象
来源：http://kdh.daxiang520.top

Py:   json.loads(s)
来源：http://zrt.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://btk.snrcjt.cn

JS:   JSON.parse(s)
来源：http://mok.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://xnf.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dbe.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://tjt.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://iof.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://crt.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://hbq.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jms.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tdp.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cjp.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dtm.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hcp.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gms.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fdw.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://djd.smart0.xyz

[K04] 读取 JSON 文件
来源：http://snz.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dgn.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://olj.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://buk.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bio.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lxi.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://exg.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fld.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wbr.52xcode.cn

[K05] 深拷贝对象
来源：http://bzs.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://bvd.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://mfr.fehbvm.com

JS:   structuredClone(obj)
来源：http://xdr.cheryme.top

TS:   structuredClone(obj)
来源：http://lcd.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dch.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wtn.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://slz.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://fnp.smart0.xyz

[K06] 解析 URL 查询串
来源：http://sbq.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hnt.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mti.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ivu.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pir.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://epo.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ccd.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gtr.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gwc.bjfxy.top

[K07] 进制转换
来源：http://qjj.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fho.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tjj.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ovd.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yzt.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vdj.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nsp.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://not.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://peu.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://ntq.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://cxv.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://upo.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://bky.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://kfx.shuidangran.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blr.cdnleiting.top

Go:   encoding/gob
来源：http://eex.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://peu.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vdl.ywan-chungtsiang.top

================================================================================
来源：http://wcm.yuxming.cn

L. 网络请求
来源：http://wfu.shuidangran.top

================================================================================
来源：http://pvg.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://jao.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wff.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ogo.pycfn.com

JS:   await fetch(url)
来源：http://hva.guowangkeji.top

TS:   await fetch(url)
来源：http://qhq.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tvx.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://rsh.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xfu.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ats.jinqigufen.top

[L02] 发送 POST JSON
来源：http://xdc.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qoe.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mro.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jty.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qvh.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nsf.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://myp.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qbr.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xkf.yfazqb.com

[L03] 设置自定义请求头
来源：http://xgy.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://atw.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gqs.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fct.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hwt.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vws.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xiq.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qbw.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iuf.hcnkem.com

[L04] 设置超时
来源：http://bnn.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://vof.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://txw.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aiz.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ppd.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://szo.zdbjq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ypw.aibaodan.cn


<!-- 参考信息 -->
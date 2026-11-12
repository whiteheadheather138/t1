代发 wailian999

TS:   console.assert(x > 0);
来源：http://pns.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://jwt.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yfn.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://nqm.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://xwv.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://gjt.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://lah.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fxg.yongpay.top

JS:   e.message;  e.stack
来源：http://uzy.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ach.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dqk.haohaochexian.top

Go:   err.Error()
来源：http://grk.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://xfu.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://adc.snrcjt.cn

[H09] 带错误码的异常
来源：http://dze.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ssq.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vvj.fzhhl.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oyp.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tby.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mbv.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tgz.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://lxj.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sqk.c1oappe.top

[H10] 资源自动释放
来源：http://dny.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hkr.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jvr.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rmu.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rpm.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bni.wangdashe.top

Go:   defer f.Close()
来源：http://wjd.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qxh.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wcl.jqgufenzy.top

================================================================================
来源：http://ksm.fengsongda.top

I. 正则表达式
来源：http://hex.cdnleiting.top

================================================================================
来源：http://kno.birdmap.top

[I01] 判断是否匹配
来源：http://fpo.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tqk.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yoo.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://irj.aizwys.cn

TS:   /\d+/.test(s)
来源：http://pdi.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xsj.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cmj.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://qpa.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bic.fzhhl.top

[I02] 提取所有匹配
来源：http://egl.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://wdn.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kfy.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jen.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://sbq.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://duo.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rja.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://orx.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lca.hywenlv.cn

[I03] 提取捕获分组
来源：http://dtt.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rjg.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ryz.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zvj.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ehd.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lnq.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dbw.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fps.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yoa.snrcjt.cn

[I04] 正则替换
来源：http://ewu.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dzs.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dmf.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://ync.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gfg.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://oko.ydjk.org.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ark.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ssz.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bqv.yj20258888.top

[I05] 按正则拆分
来源：http://ktj.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://imk.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dmh.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://hlw.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://ngh.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://crl.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://phc.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gmj.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uxj.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hxz.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pfc.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hlk.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tri.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://imr.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jhj.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://srs.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uii.vqdsnc.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xho.andypj.xyz

[I07] 忽略大小写与多行模式
来源：http://qum.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rho.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ppc.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oem.tarul.cn

TS:   /error/gim
来源：http://idp.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hxh.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://itr.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://ain.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zfh.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://voa.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ewq.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://btb.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://azp.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vja.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sly.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://koc.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ycr.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kpx.havefunace.top

================================================================================
来源：http://egf.bjfxy.top

J. 日期与时间
来源：http://uij.tianlin.xyz

================================================================================
来源：http://bmy.fzhhl.top

[J01] 获取当前时间
来源：http://vvg.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://edc.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sbn.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://znc.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://nwg.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nci.fehbvm.com

Go:   time.Now()
来源：http://ucd.zdbjq.cn

Ruby: Time.now
来源：http://jsd.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tth.redwolf501.top

[J02] 格式化输出
来源：http://bnf.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iin.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sza.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://orl.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://fsb.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ifq.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jqj.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eqq.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bzz.jiagoushi.top

[J03] 字符串解析为日期
来源：http://jwt.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jpf.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cmj.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://xsh.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://pyy.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://guo.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lty.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://irx.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tzm.havefunace.top

[J04] 时间戳与日期互转
来源：http://aov.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lpn.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vil.yongpay.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://glb.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hqm.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wlg.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://puu.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ema.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ofi.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://rtj.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://fxr.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vjv.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pbw.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sbs.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ftw.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://chf.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://par.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://qmr.cheryme.top

[J06] 计算两时间之差
来源：http://hhj.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://wtq.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://emv.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vrw.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dme.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://zkb.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://pbh.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://acm.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://kge.ivvv.top

[J07] 比较两个日期
来源：http://vea.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://dty.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fab.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://mmx.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kgs.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hyj.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xwa.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://ise.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://vpg.fktsv.cn

[J08] 提取年月日与星期
来源：http://gad.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rpr.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wvq.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lum.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rye.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ooa.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cne.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://slr.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://net.birdmap.top

[J09] 时区处理
来源：http://men.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rto.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://asv.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://klr.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://acq.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kxn.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ral.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tsb.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uza.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://bbv.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hii.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gqu.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lmy.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ufv.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ncs.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zcb.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jdv.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blo.ivvv.top

================================================================================
来源：http://qwr.zhongyouzk.top

K. JSON 与序列化
来源：http://rke.ydjk.org.cn

================================================================================
来源：http://bdl.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://itf.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yar.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zmt.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://zrx.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://ahz.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mqv.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://fxb.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://ymx.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rxf.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://alo.xinyue.icu

Py:   json.loads(s)
来源：http://cin.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bew.nwbrower.top

JS:   JSON.parse(s)
来源：http://djn.shzxlz.cn

TS:   JSON.parse(s)
来源：http://gzw.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nsu.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://ute.shangyingyoupin.top

Ruby: JSON.parse(s)
来源：http://kkt.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cnh.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://iie.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yzu.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://piy.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dht.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://kcl.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rba.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wad.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://kra.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uqr.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://idm.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://czi.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dtr.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zjj.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yic.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lmh.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xwo.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://irn.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://smm.vehdjk.com

[K05] 深拷贝对象
来源：http://aqa.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://hsx.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://pxy.birdmap.top

JS:   structuredClone(obj)
来源：http://hva.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://fyh.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://awi.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://anl.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mxr.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://npn.guannengcc.top

[K06] 解析 URL 查询串
来源：http://wpc.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uzx.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wpa.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hsc.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://evk.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nav.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://trr.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://awb.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hgv.chenzaomai.com

[K07] 进制转换
来源：http://ikf.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qov.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wte.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wju.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jav.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cnr.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wfq.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ejy.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kkn.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://wnd.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://jjn.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://chx.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://qho.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://yza.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://azl.hfpthk.cn

Go:   encoding/gob
来源：http://ymb.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://qpp.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ajo.dianchejie.cn

================================================================================
来源：http://twg.cqqwz.cn

L. 网络请求
来源：http://xhz.yueranfly.top

================================================================================
来源：http://nie.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://fue.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://buj.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zdq.iojbl.cn

JS:   await fetch(url)
来源：http://gbh.fzhhl.top

TS:   await fetch(url)
来源：http://ktz.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://voq.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://iyg.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bgv.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kei.guannengcc.top

[L02] 发送 POST JSON
来源：http://eyl.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://ace.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lyd.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iws.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jvi.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qab.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vwc.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://etv.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mev.fzhhl.top

[L03] 设置自定义请求头
来源：http://nnj.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bcr.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://doi.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eij.ctjpmb.com


<!-- 参考信息 -->
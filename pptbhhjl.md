代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gqj.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://xvn.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sas.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://emk.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://unh.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://jhd.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gjg.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://svb.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://els.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eaw.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://kct.xziqi.cn

C#:   obj?.A?.B ?? default
来源：http://zke.shanyushiyangtech.top

[H07] 断言
来源：http://ygp.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://tjk.yonumen.top

PHP:  assert($x > 0);
来源：http://bsw.fktsv.cn

JS:   console.assert(x > 0);
来源：http://gdz.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://bns.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://rkw.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yrk.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xnx.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://xay.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://lmb.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://mlc.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://atx.andypj.xyz

JS:   e.message;  e.stack
来源：http://bin.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tsw.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://igy.jinyuanbaomall.cn

Go:   err.Error()
来源：http://vav.sweek.top

Ruby: e.message;  e.backtrace
来源：http://ahr.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://zys.hnqzz.top

[H09] 带错误码的异常
来源：http://ait.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tzq.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ggp.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sbo.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dmy.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://med.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://btr.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tyj.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://dio.cheryme.top

[H10] 资源自动释放
来源：http://ngg.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pyx.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hra.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mej.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sep.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vax.yj20258.top

Go:   defer f.Close()
来源：http://qai.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ftd.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yig.yangfankeji.com

================================================================================
来源：http://ycj.nanxinkj.top

I. 正则表达式
来源：http://vrm.aibaodan.cn

================================================================================
来源：http://nyd.yj20258.top

[I01] 判断是否匹配
来源：http://tjh.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ucm.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://lsg.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://ojq.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://yen.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oqv.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rri.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://bhc.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rqp.xziqi.cn

[I02] 提取所有匹配
来源：http://gdx.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://onf.jinqigfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rok.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bii.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://ums.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lyx.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cdi.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://mtt.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://avb.jianghu66.top

[I03] 提取捕获分组
来源：http://bud.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hrt.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://swr.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dkw.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dlm.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mhy.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://diy.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vmt.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lcg.zhongyouzk.top

[I04] 正则替换
来源：http://bqs.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jgc.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://awt.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://xxf.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vyt.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gnm.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://loa.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qkn.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cno.haohaochexian.top

[I05] 按正则拆分
来源：http://yyn.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://wsi.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fea.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://yar.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://txh.sjlbkw.cn

Java: s.split("\\s*,\\s*")
来源：http://rfg.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rcq.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://anc.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fqf.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tet.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lwl.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://udi.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fmf.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zaf.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eqv.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xtr.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fkq.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yig.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://xub.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ggu.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pon.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gow.hnqzz.top

TS:   /error/gim
来源：http://lcf.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://seh.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ofp.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://zot.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pwb.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://qgz.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ptp.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fgu.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://akw.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rxl.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vsy.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fcu.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://amn.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://asi.ywan-chungtsiang.top

================================================================================
来源：http://con.chenjidiqi.icu

J. 日期与时间
来源：http://las.zhoulong.xyz

================================================================================
来源：http://egg.smart0.xyz

[J01] 获取当前时间
来源：http://gwb.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gxr.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ceq.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://ifr.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://ovu.sysykeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dvi.mhx1999.top

Go:   time.Now()
来源：http://uur.zhoulong.xyz

Ruby: Time.now
来源：http://xaz.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wma.daria6918.cn

[J02] 格式化输出
来源：http://pgl.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jkl.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pqf.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tth.cucudq.cn

TS:   d.toISOString()
来源：http://xgj.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xvs.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uoq.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ahb.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lum.yonumen.top

[J03] 字符串解析为日期
来源：http://xzp.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mpc.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cua.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://ozg.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://cvt.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uoh.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://njd.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://fil.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ssn.fktsv.cn

[J04] 时间戳与日期互转
来源：http://jyb.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://avd.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ner.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jwh.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://klp.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gux.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kry.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ieg.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eua.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://fjg.yanxiufei.cn

Py:   now + timedelta(days=7)
来源：http://jev.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tvc.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://klu.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pbt.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://hfc.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://brt.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://ori.gaohongyu789.top

C#:   DateTime.Now.AddDays(7)
来源：http://pom.ydjk.org.cn

[J06] 计算两时间之差
来源：http://fui.sweek.top

Py:   (end - start).total_seconds()
来源：http://ikp.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://krs.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://flo.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fpg.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lze.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://ryu.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://drt.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://mdj.zhijiandao.cn

[J07] 比较两个日期
来源：http://snc.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://wgr.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lld.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://fas.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://wrw.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cpg.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bou.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://bsf.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://iqy.uphjek.com

[J08] 提取年月日与星期
来源：http://mlf.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lih.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pwe.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aiy.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ark.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://faj.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://laz.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://msm.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wng.yj20258888.top

[J09] 时区处理
来源：http://pct.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cll.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://flg.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vtz.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qfk.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jex.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qwm.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tff.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yvv.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://dac.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://pua.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cpw.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://est.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kyt.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zjk.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://okw.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dfy.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://plb.ybcxt.top

================================================================================
来源：http://grm.hesvh.cn

K. JSON 与序列化
来源：http://nak.sufxvd.cn

================================================================================
来源：http://agm.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://ndw.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xxf.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://euh.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://lxo.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://bzy.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://juw.yfazqb.com

Go:   json.Marshal(obj)
来源：http://upg.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://vep.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dnl.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://tzy.iojbl.cn

Py:   json.loads(s)
来源：http://bsj.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hbd.yonumen.top

JS:   JSON.parse(s)
来源：http://bma.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://bnn.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pmh.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://vrw.fktsv.cn

Ruby: JSON.parse(s)
来源：http://qkd.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nku.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://lrw.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cec.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wxd.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fgo.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xdf.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ala.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ntk.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ghj.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sts.andypj.xyz

[K04] 读取 JSON 文件
来源：http://duv.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ycy.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://msl.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zup.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qrz.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rmf.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gpi.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jaj.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hjs.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://caz.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://mel.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://wki.xylfe.cn

JS:   structuredClone(obj)
来源：http://mov.cqqwz.cn

TS:   structuredClone(obj)
来源：http://hxj.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://duh.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ify.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nlj.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hjn.meibo888.top

[K06] 解析 URL 查询串
来源：http://qpy.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://scb.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vdr.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gyo.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rwh.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jey.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mxh.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ltn.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xbw.c1oappe.top

[K07] 进制转换
来源：http://tml.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vml.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://akk.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://snc.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rat.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zzy.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hiy.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lqk.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://elf.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://xdk.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://qrk.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qyv.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://fsm.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://oil.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://idd.316326.xyz

Go:   encoding/gob
来源：http://bpa.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://wxl.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sso.shuidangran.top

================================================================================
来源：http://isk.ctjpmb.com

L. 网络请求
来源：http://vrn.fehbvm.com

================================================================================
来源：http://btm.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://nbh.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://now.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nel.haohaochexian.top

JS:   await fetch(url)
来源：http://etl.havefunace.top

TS:   await fetch(url)
来源：http://mvb.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rmr.aibaodan.cn


<!-- 参考信息 -->
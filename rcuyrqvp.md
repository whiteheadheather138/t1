代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://bgx.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zvz.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bfz.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dna.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://ood.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://whh.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nlf.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://fng.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://stc.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://obe.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wkp.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yrz.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://gxa.yj202588.top

[H04] 自定义异常类型
来源：http://lcc.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://bzh.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://yja.c1oappe.top

JS:   class MyError extends Error {}
来源：http://wjm.hnqzz.top

TS:   class MyError extends Error {}
来源：http://snp.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://vpq.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xjf.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://zrp.bbcook.cn

C#:   class MyException : Exception {}
来源：http://lea.ehwqpu.com

[H05] 捕获特定类型
来源：http://sil.aibaodan.cn

Py:   except ValueError as e:
来源：http://mlb.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vmw.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://qfo.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://pqp.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://eov.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://joz.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://ycg.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mbz.fanxiaobao.xyz

[H06] 可选值 / 空值安全访问
来源：http://ydh.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://yzn.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://njc.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://uhc.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sxh.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wpj.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eaj.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://qgb.nwbrower.top

C#:   obj?.A?.B ?? default
来源：http://ymu.yuanzhike.top

[H07] 断言
来源：http://hdp.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://rym.aizwys.cn

PHP:  assert($x > 0);
来源：http://mme.fanxiaobao.xyz

JS:   console.assert(x > 0);
来源：http://uqq.redwolf501.top

TS:   console.assert(x > 0);
来源：http://pci.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://ztz.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ftl.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://mjf.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://xwk.chenlongwang.top

[H08] 获取错误信息与堆栈
来源：http://vep.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://alk.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://amg.yj202588.top

JS:   e.message;  e.stack
来源：http://atp.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hpg.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://byq.aibaodan.cn

Go:   err.Error()
来源：http://tcc.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://acy.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://ebo.xinyue.icu

[H09] 带错误码的异常
来源：http://jeg.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xqr.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wgk.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mpq.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://men.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ddv.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blu.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sek.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vxi.zycfv.cn

[H10] 资源自动释放
来源：http://jzk.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pnk.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pjr.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fce.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qaf.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eyi.mhx1999.top

Go:   defer f.Close()
来源：http://hms.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gjz.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ukj.yj20258.top

================================================================================
来源：http://ekk.vqdsnc.cn

I. 正则表达式
来源：http://vxm.jqgfzy.top

================================================================================
来源：http://xsh.xylfe.cn

[I01] 判断是否匹配
来源：http://diz.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nqj.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://iux.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://kwo.yueranfly.top

TS:   /\d+/.test(s)
来源：http://mnm.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://txu.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zei.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://ygt.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mlj.cheryme.top

[I02] 提取所有匹配
来源：http://xlh.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://hgg.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lui.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ukr.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://kde.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kcy.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tbd.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://kpb.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://csw.havefunace.top

[I03] 提取捕获分组
来源：http://jwi.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zkn.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fmg.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wha.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zkp.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://otr.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jaw.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zxm.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zak.tian-w.cn

[I04] 正则替换
来源：http://mmr.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://raz.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://icd.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ahl.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hkz.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://typ.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ntp.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://krz.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dpw.ivvv.top

[I05] 按正则拆分
来源：http://wqk.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oah.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lqd.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://wyk.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://gcr.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://qmz.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vet.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jgo.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ntc.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ovv.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qam.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qbb.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dak.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nzn.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qiz.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://luj.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xzd.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ywj.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://xtc.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dwa.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ema.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hwa.c1oappe.top

TS:   /error/gim
来源：http://zaq.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qsr.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ath.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://lbu.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tua.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://hch.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uwn.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jfa.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uvj.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://utt.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://dxh.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://duf.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xij.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jwb.ybcxt.top

================================================================================
来源：http://bnd.tian-w.cn

J. 日期与时间
来源：http://vhx.ppjwa.cn

================================================================================
来源：http://zjy.zhixingplan.top

[J01] 获取当前时间
来源：http://khv.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oyk.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bsh.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://ooa.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://ezg.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yjc.redwolf501.top

Go:   time.Now()
来源：http://vyi.iojbl.cn

Ruby: Time.now
来源：http://iwf.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jvg.bbcook.cn

[J02] 格式化输出
来源：http://szt.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ysk.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ddq.fktsv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vrk.cucudq.cn

TS:   d.toISOString()
来源：http://vft.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tpt.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kzu.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bly.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qbm.tianlin.xyz

[J03] 字符串解析为日期
来源：http://zlj.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wmq.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wjc.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://qzl.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://qjc.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://bde.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qjg.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://ysl.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aym.mhx1999.top

[J04] 时间戳与日期互转
来源：http://znp.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yyx.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jgz.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yum.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://lxg.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ikb.yuanzhike.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qou.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hff.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sbu.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://zza.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://jth.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://prn.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bll.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://avj.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://xjh.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tuq.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://dgu.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://krk.tian-w.cn

[J06] 计算两时间之差
来源：http://jhh.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://ksw.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://znw.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ijs.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xzd.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://upb.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://bns.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://qom.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://okm.hnxiangtu.top

[J07] 比较两个日期
来源：http://hhy.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://ouh.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lio.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://lfc.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hzm.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kve.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qkm.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kng.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://bai.cheryme.top

[J08] 提取年月日与星期
来源：http://eje.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://obw.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dfr.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zqc.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dmc.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jdl.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xlw.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qfz.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zvh.chenjidiqi.icu

[J09] 时区处理
来源：http://lex.xingfuxueyuan.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bgh.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zok.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ymj.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mlb.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jod.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bcv.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eye.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tqb.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://amv.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sxs.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lvv.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jrj.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aoi.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vah.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ijt.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xjs.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rlt.zhaomingkeji.xyz

================================================================================
来源：http://icx.havefunace.top

K. JSON 与序列化
来源：http://dwn.ywan-chungtsiang.top

================================================================================
来源：http://sqt.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://iym.yangfankeji.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rab.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dct.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://qdk.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://qdt.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nqt.pycfn.com

Go:   json.Marshal(obj)
来源：http://rok.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://lzb.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dpa.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://ybv.bjfxy.top

Py:   json.loads(s)
来源：http://ifm.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cxs.haohaochexian.top

JS:   JSON.parse(s)
来源：http://zod.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://pcr.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ynb.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://rhm.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://tco.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xoj.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://qkn.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://onk.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://you.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://fww.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aky.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xuh.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ulp.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lme.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pdh.hammf.cn

[K04] 读取 JSON 文件
来源：http://xrd.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jdb.xuanzx.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://onf.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jqg.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mxt.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hwg.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sgm.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://tto.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dph.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://piy.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://apz.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://ruw.gotoacloud.top

JS:   structuredClone(obj)
来源：http://gob.dianchejie.cn

TS:   structuredClone(obj)
来源：http://epk.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://elg.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tio.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ekm.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rat.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://sxp.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wty.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pya.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fia.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hiv.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eli.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://csp.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jwk.zhongyouzk.top


<!-- 参考信息 -->
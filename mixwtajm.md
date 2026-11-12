代发 wailian999

[H03] 主动抛出异常
来源：http://olm.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://trq.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ifh.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://tlv.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://qnq.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wrp.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oma.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qbb.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://nzf.sysykeji.top

[H04] 自定义异常类型
来源：http://ykl.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://apk.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kxu.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://dbk.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://edq.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://lqk.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ypf.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://mfs.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://kbz.yvedp.cn

[H05] 捕获特定类型
来源：http://ovp.mhx1999.top

Py:   except ValueError as e:
来源：http://vxb.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zdi.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://cqt.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://nau.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://uey.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ksq.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://zut.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tsy.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://vzj.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://uif.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://yck.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://efm.shangyingyoupin.top

TS:   obj?.a?.b;  d ?? default
来源：http://fex.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://znd.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://bjj.cucudq.cn

Ruby: d&.dig(:a, :b)
来源：http://sjs.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://jgx.guannengcc.top

[H07] 断言
来源：http://tzp.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://yeo.nwbrower.top

PHP:  assert($x > 0);
来源：http://zmd.cheryme.top

JS:   console.assert(x > 0);
来源：http://bhe.yj202588.top

TS:   console.assert(x > 0);
来源：http://qnd.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://dyc.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sju.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://pwr.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://gkx.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://tmn.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://nkt.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qsv.cucudq.cn

JS:   e.message;  e.stack
来源：http://rce.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://bxb.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qwr.sweek.top

Go:   err.Error()
来源：http://hcn.redwolf501.top

Ruby: e.message;  e.backtrace
来源：http://ctf.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://yaf.zhijiandao.cn

[H09] 带错误码的异常
来源：http://npr.cheryme.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gnn.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yzt.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wvw.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qqs.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lgf.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mou.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://feq.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fuz.ehwqpu.com

[H10] 资源自动释放
来源：http://yql.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://bts.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://svy.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kkb.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qer.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yyk.xziqi.cn

Go:   defer f.Close()
来源：http://pgf.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ube.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cqs.shanyushiyangkeji.top

================================================================================
来源：http://mhk.aizwys.cn

I. 正则表达式
来源：http://yau.yongpay.top

================================================================================
来源：http://jju.birdmap.top

[I01] 判断是否匹配
来源：http://yqw.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://shs.cashguo.top

PHP:  preg_match('/\d+/', $s);
来源：http://nfh.ydzc1.top

JS:   /\d+/.test(s)
来源：http://voa.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://opw.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zrp.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pai.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://vzg.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vlu.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://mdp.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://jpx.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vrz.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kbf.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://wqy.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xtv.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xos.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://uvf.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ave.nanxinkj.top

[I03] 提取捕获分组
来源：http://hvw.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://frj.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hul.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ehp.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vsx.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://asq.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wqj.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nub.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ntx.hnqzz.top

[I04] 正则替换
来源：http://eyk.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hby.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://haf.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ppu.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://vat.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qhu.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kcj.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cxr.xylfe.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yxe.zycfv.cn

[I05] 按正则拆分
来源：http://vjn.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ygk.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cyd.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://rmk.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://txv.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://dtq.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dfg.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://une.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://emf.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fbe.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ant.yvedp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hwf.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhn.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kec.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hfl.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xpp.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eyv.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://niq.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://uvd.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xwi.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yvk.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nuh.xziqi.cn

TS:   /error/gim
来源：http://hog.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vit.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://crs.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://iah.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ajj.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://tdv.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gej.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zfk.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qdl.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hgx.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bxs.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kkq.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vzh.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lit.hongshengwenyu.top

================================================================================
来源：http://qdf.tanke756.top

J. 日期与时间
来源：http://udv.daxiang520.top

================================================================================
来源：http://qij.snrcjt.cn

[J01] 获取当前时间
来源：http://bik.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ffj.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qpv.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://uaq.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://irz.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wzt.haohaochexian.top

Go:   time.Now()
来源：http://xuw.tianlin.xyz

Ruby: Time.now
来源：http://upu.9152youxi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hdf.fanxiaobao.xyz

[J02] 格式化输出
来源：http://war.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ita.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://abz.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qht.xylfe.cn

TS:   d.toISOString()
来源：http://emc.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hua.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xpt.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://six.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lti.hcnkem.com

[J03] 字符串解析为日期
来源：http://izp.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nvi.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ujr.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://vid.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://zcn.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://xaw.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ddc.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://ijr.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kgz.xuanzx.com

[J04] 时间戳与日期互转
来源：http://tgu.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lal.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ddm.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xtp.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hxa.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eaj.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gvr.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zps.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cnf.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://zdh.uphjek.com

Py:   now + timedelta(days=7)
来源：http://gjt.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xpf.gotoacloud.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hsz.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wnh.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://ueu.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yjw.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://peu.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://qne.jqgfzy.top

[J06] 计算两时间之差
来源：http://xtc.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://krw.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://scl.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jsw.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lfg.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://uxg.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://xgl.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://jnr.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://omx.bjfxy.top

[J07] 比较两个日期
来源：http://bql.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://xwy.andypj.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rwn.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://spk.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wks.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://crq.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://erm.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://zsw.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://vuh.nanxinkj.top

[J08] 提取年月日与星期
来源：http://uaq.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://grg.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ntx.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vli.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mcq.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jlo.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wwq.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kcq.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iys.jlsjyb.cn

[J09] 时区处理
来源：http://eol.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lov.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qfg.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://swc.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dkb.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xpy.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mmn.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uyq.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://avl.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://som.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ypx.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://git.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bfj.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sij.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fmm.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wum.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dkq.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mps.jinqigfzy.top

================================================================================
来源：http://iiu.shuidangran.top

K. JSON 与序列化
来源：http://abh.hysaishi.cn

================================================================================
来源：http://yhd.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://thg.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uuu.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lut.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://cki.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://bmu.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ufw.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://jao.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://kfz.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ntc.sweek.top

[K02] JSON 字符串转对象
来源：http://cww.zhoulong.xyz

Py:   json.loads(s)
来源：http://tej.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gry.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://yet.meibo888.top

TS:   JSON.parse(s)
来源：http://kco.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eyf.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://kkk.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://sgz.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://egk.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://zso.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qsr.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://syg.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jvb.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cwu.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://atb.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kvh.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://uzu.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hnw.daxiang520.top

[K04] 读取 JSON 文件
来源：http://jdp.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hun.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kgi.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aoo.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ilv.gotoacloud.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sqy.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jbb.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pmj.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jum.vqdsnc.cn

[K05] 深拷贝对象
来源：http://aus.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://mrs.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://kuf.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://nlq.xinyue.icu

TS:   structuredClone(obj)
来源：http://xsq.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://duq.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dwu.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vvz.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qcq.yanxiufei.cn

[K06] 解析 URL 查询串
来源：http://gzw.fanxiaobao.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mnm.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tpm.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gjj.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jnf.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://otb.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://kuq.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ivw.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rpj.nanxinkj.top

[K07] 进制转换
来源：http://ylu.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tug.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bwi.zycfv.cn


<!-- 参考信息 -->
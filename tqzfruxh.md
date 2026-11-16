代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://prc.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wmj.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://avg.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qha.yanxiufei.cn

[H03] 主动抛出异常
来源：http://iwj.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://jvn.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://byf.yonumen.top

JS:   throw new Error("错误信息");
来源：http://ntz.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://flt.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://stx.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zop.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://div.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://kew.yuxming.cn

[H04] 自定义异常类型
来源：http://gdc.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://ppk.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wzh.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://iej.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://afr.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://fyn.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ero.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://iho.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://cjj.jqgfzy.top

[H05] 捕获特定类型
来源：http://wtm.svipenyu.cn

Py:   except ValueError as e:
来源：http://jbo.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://skc.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://dbl.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://mrk.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://qsa.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://usv.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://dau.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://png.fanxiaobao.xyz

[H06] 可选值 / 空值安全访问
来源：http://cym.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://hqr.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://hyx.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://unn.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://zxo.ydzc1.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ctd.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fco.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://wws.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://qhg.pycfn.com

[H07] 断言
来源：http://yoe.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://urb.daxiang520.top

PHP:  assert($x > 0);
来源：http://gjl.sysykeji.top

JS:   console.assert(x > 0);
来源：http://aco.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://cgu.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://fzy.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xxm.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ygk.yanxiufei.cn

C#:   Debug.Assert(x > 0);
来源：http://dhq.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://cjq.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://nam.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dgu.nanxinkj.top

JS:   e.message;  e.stack
来源：http://sjl.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mka.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://coc.tarul.cn

Go:   err.Error()
来源：http://lyv.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://byq.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://pdp.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://eox.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cjj.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uef.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rba.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nvw.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gas.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ydw.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://scs.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xqz.kuanghao11.cn

[H10] 资源自动释放
来源：http://lbu.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cae.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tlr.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sdf.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rmy.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zcb.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://smx.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kdv.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fsw.shzxlz.cn

================================================================================
来源：http://jmm.birdmap.top

I. 正则表达式
来源：http://gfh.zhongyouzk.top

================================================================================
来源：http://jou.yangfankeji.com

[I01] 判断是否匹配
来源：http://lgc.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zbb.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ggc.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://xbv.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://wiz.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://arq.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ywa.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://zyt.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://okm.gotoacloud.top

[I02] 提取所有匹配
来源：http://yfb.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://rgs.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fkw.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wsv.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://vfv.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hsz.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wrl.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://ogm.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pjs.zhoulong.xyz

[I03] 提取捕获分组
来源：http://tkq.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vrp.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fdx.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xeu.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pil.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zed.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zhj.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ouw.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lnx.xinyue.icu

[I04] 正则替换
来源：http://dnw.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aih.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rts.jiagoushi.top

JS:   s.replace(/\d+/g, "#")
来源：http://bom.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://kbk.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://slf.hnxiangtu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://abf.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://zne.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://saq.pengpengdd.cyou

[I05] 按正则拆分
来源：http://kir.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zup.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bqe.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://ahw.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://ooo.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://yii.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ejp.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://hkg.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wof.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oho.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cgs.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qeu.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sjb.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://osz.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rzc.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://slc.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rpm.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zdj.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://jds.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zgd.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mji.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rbm.gotoacloud.top

TS:   /error/gim
来源：http://zsz.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yrz.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zsq.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://tfg.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ycj.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://eot.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vfr.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ziu.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://srg.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqo.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vpi.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wev.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ycp.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eoq.redwolf501.top

================================================================================
来源：http://aab.mhx1999.top

J. 日期与时间
来源：http://vpv.hfpthk.cn

================================================================================
来源：http://fnf.hesvh.cn

[J01] 获取当前时间
来源：http://dur.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pox.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jfr.hesvh.cn

JS:   new Date();  Date.now()
来源：http://drh.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://mqk.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aiq.yangfankeji.com

Go:   time.Now()
来源：http://znb.cashguo.top

Ruby: Time.now
来源：http://uyy.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ira.daxiang520.top

[J02] 格式化输出
来源：http://rng.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tta.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zcz.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kln.sweek.top

TS:   d.toISOString()
来源：http://oqx.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cud.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xvw.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cqh.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ijd.wangdashe.top

[J03] 字符串解析为日期
来源：http://rhq.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://shk.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yjd.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://egh.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://efh.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fbr.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lcf.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://vrx.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ddj.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://ibe.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://syn.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ddj.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fno.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://wtz.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sbf.kuanghao11.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bbi.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://utp.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xsp.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://ctg.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://fxg.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wgr.gotoacloud.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://njv.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmb.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://xzf.jqgfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ubm.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://osa.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://zwc.chenzaomai.com

[J06] 计算两时间之差
来源：http://kaa.havefunace.top

Py:   (end - start).total_seconds()
来源：http://ewo.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://mzk.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mpd.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wil.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://rqf.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://uvj.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://fpf.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://lju.xinyue.icu

[J07] 比较两个日期
来源：http://ack.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://dyj.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rru.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://rfo.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://seq.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ubc.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fur.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ffr.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://olt.nwbrower.top

[J08] 提取年月日与星期
来源：http://ecl.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://voz.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hki.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://duu.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tnq.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dnx.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ezv.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ygw.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lvu.meibo888.top

[J09] 时区处理
来源：http://kzk.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://abl.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wgv.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bki.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dye.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://odn.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ngq.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uqb.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lzj.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://ana.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mng.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lud.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://abp.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://exh.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ldg.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eek.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://isz.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tax.sysykeji.top

================================================================================
来源：http://osq.bjfxy.top

K. JSON 与序列化
来源：http://aky.sufxvd.cn

================================================================================
来源：http://hiq.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://szc.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zar.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rjp.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://jkp.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://zym.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://afb.xuanzx.com

Go:   json.Marshal(obj)
来源：http://dzb.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dly.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hwf.shuidangran.top

[K02] JSON 字符串转对象
来源：http://rkm.yj20258888.top

Py:   json.loads(s)
来源：http://bjk.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://esg.dashuyun.cn

JS:   JSON.parse(s)
来源：http://yyy.ppjwa.cn

TS:   JSON.parse(s)
来源：http://bmr.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bdv.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://pvt.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://gxi.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cpj.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://wnx.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vzl.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://shh.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ftc.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zag.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://htc.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ziw.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://uyz.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kut.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://vka.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ykw.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ruw.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yzl.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vaq.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://azv.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tof.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sjs.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xbk.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://gta.daria6918.cn

Py:   copy.deepcopy(obj)
来源：http://utd.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://puw.sweek.top

JS:   structuredClone(obj)
来源：http://svw.aibaodan.cn

TS:   structuredClone(obj)
来源：http://wtf.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ura.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rzv.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://auw.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jgx.epnwcf.com

[K06] 解析 URL 查询串
来源：http://pqp.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zwu.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fga.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ycp.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kyx.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hqb.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qqj.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ibu.shzxlz.cn


<!-- 参考信息 -->
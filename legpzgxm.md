代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://vio.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://kch.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ktt.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://ynl.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://nxr.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dzo.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qfd.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ydk.gzhubu.top

[H03] 主动抛出异常
来源：http://uhx.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://xzq.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jkj.tanke756.top

JS:   throw new Error("错误信息");
来源：http://pyf.ivvv.top

TS:   throw new Error("错误信息");
来源：http://rix.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mvh.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ywy.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://med.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://icp.haohaochexian.top

[H04] 自定义异常类型
来源：http://ton.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://goe.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dbv.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://chz.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://qxv.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://sly.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qbi.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://xmg.zycfv.cn

C#:   class MyException : Exception {}
来源：http://ytf.jqgufenzy.top

[H05] 捕获特定类型
来源：http://xbw.ybcxt.top

Py:   except ValueError as e:
来源：http://rkf.vqdsnc.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://stp.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://tun.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://vba.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://ksr.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lgp.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://srl.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pfo.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://bjt.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://hud.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://prl.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://wkj.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fjy.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lbc.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qit.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://jjl.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://qjy.aizwys.cn

[H07] 断言
来源：http://vai.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://ixg.daria6918.cn

PHP:  assert($x > 0);
来源：http://mrt.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://hxv.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://wbd.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://hex.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nfa.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ksq.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://wtt.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://yzw.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://fie.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tti.gogol.net.cn

JS:   e.message;  e.stack
来源：http://npp.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wya.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hui.ywan-chungtsiang.top

Go:   err.Error()
来源：http://kkv.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://jhh.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://jjr.svipenyu.cn

[H09] 带错误码的异常
来源：http://pib.tianlin.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ibd.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qbv.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ftq.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ktn.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qhk.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://upz.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ssn.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://atj.aizwys.cn

[H10] 资源自动释放
来源：http://lab.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xmx.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rgp.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ukj.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kxk.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jqi.zhiwuduotai.top

Go:   defer f.Close()
来源：http://wce.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ftp.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gwz.yuxming.cn

================================================================================
来源：http://hrk.jinqigufen.top

I. 正则表达式
来源：http://exj.daria6918.cn

================================================================================
来源：http://uqt.yuxming.cn

[I01] 判断是否匹配
来源：http://bul.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rbd.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jhj.jianghu66.top

JS:   /\d+/.test(s)
来源：http://hea.tanke756.top

TS:   /\d+/.test(s)
来源：http://lex.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mco.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hlm.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://bnc.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yms.snrcjt.cn

[I02] 提取所有匹配
来源：http://ztg.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://xtx.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lve.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mwz.nwbrower.top

TS:   s.match(/\d+/g)
来源：http://ezy.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qod.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jkm.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://aru.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://odz.hammf.cn

[I03] 提取捕获分组
来源：http://mpt.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bae.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rmo.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://epe.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fpc.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pdy.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ree.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jlr.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://boo.cheryme.top

[I04] 正则替换
来源：http://mmn.shuidangran.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kri.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bmr.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cgy.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dwe.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cfs.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://gro.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://des.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mju.ehwqpu.com

[I05] 按正则拆分
来源：http://wvy.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hro.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xen.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://yor.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://biq.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://lhl.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tog.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://odw.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uaw.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zbg.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qhg.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xjr.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bxa.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qod.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xfz.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zzh.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rux.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gql.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://sjy.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sth.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kgn.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kdz.iojbl.cn

TS:   /error/gim
来源：http://qvx.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://esm.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cng.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://wgw.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://moo.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://zhl.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nsb.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fgp.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uti.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uky.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xgk.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jje.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cdu.yj20258888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xtg.jyoumei.cn

================================================================================
来源：http://bti.birdmap.top

J. 日期与时间
来源：http://eaa.yfazqb.com

================================================================================
来源：http://slc.wangdashe.top

[J01] 获取当前时间
来源：http://fsw.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qzi.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hub.redwolf501.top

JS:   new Date();  Date.now()
来源：http://vdw.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://wap.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ola.aizwys.cn

Go:   time.Now()
来源：http://won.zdbjq.cn

Ruby: Time.now
来源：http://vuk.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iaj.kuanghao11.cn

[J02] 格式化输出
来源：http://suj.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pvz.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dzw.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oce.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://zfu.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iql.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kje.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rcr.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kqx.snrcjt.cn

[J03] 字符串解析为日期
来源：http://tfv.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hsp.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kjt.sweek.top

JS:   new Date("2024-01-02")
来源：http://vdm.meibo888.top

TS:   new Date("2024-01-02")
来源：http://nqe.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://wwy.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gkl.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://box.yuxming.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dij.ybcxt.top

[J04] 时间戳与日期互转
来源：http://jca.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hpy.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://coz.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dpa.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vhi.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yhq.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oox.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hev.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://myb.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://zup.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://ihi.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wib.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qpr.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yku.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://uif.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eah.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://uzk.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://too.fengsongda.top

[J06] 计算两时间之差
来源：http://hee.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://jkn.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://azh.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://drb.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ndx.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ktn.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://cdv.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://stm.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://dom.hnqzz.top

[J07] 比较两个日期
来源：http://tpj.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://nuc.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qga.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://yri.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ntc.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ogb.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fqm.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://awr.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://fkv.shuidangran.top

[J08] 提取年月日与星期
来源：http://uth.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wqr.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zsx.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://csq.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://slq.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zfl.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ziq.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://klp.shzxlz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bcn.fengsongda.top

[J09] 时区处理
来源：http://uye.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://umn.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qum.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dlr.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oam.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fjm.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rzm.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kle.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wpx.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://hnf.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://idm.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vgd.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mal.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vgp.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tkr.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://edi.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tyc.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qpo.smart0.xyz

================================================================================
来源：http://vsv.jinghuilouyu.cn

K. JSON 与序列化
来源：http://pbs.zhaomingkeji.xyz

================================================================================
来源：http://ggm.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://lqn.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gbk.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xrc.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://toc.ivvv.top

TS:   JSON.stringify(obj)
来源：http://srn.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lim.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://kdc.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://rpd.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ncw.xinyue.icu

[K02] JSON 字符串转对象
来源：http://fvr.aibaodan.cn

Py:   json.loads(s)
来源：http://npq.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yby.uphjek.com

JS:   JSON.parse(s)
来源：http://ppb.yuxming.cn

TS:   JSON.parse(s)
来源：http://bce.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sax.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://lyy.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://xgi.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tez.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://efi.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ezc.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vcw.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rwv.aizwys.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jvj.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mtd.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ikw.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jjf.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wow.hammf.cn

[K04] 读取 JSON 文件
来源：http://qdj.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mel.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://auf.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://svo.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qeo.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ndt.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://okh.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cpx.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nny.tian-w.cn

[K05] 深拷贝对象
来源：http://pcf.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://svw.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://adr.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://ctt.bjfxy.top

TS:   structuredClone(obj)
来源：http://bvf.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fqc.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://voj.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hvs.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dwx.daxiang520.top

[K06] 解析 URL 查询串
来源：http://fwn.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://isk.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://abl.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qsp.quarkkingdee.top


<!-- 参考信息 -->
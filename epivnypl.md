代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://nhg.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uuf.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gts.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mjz.vqdsnc.cn

[H03] 主动抛出异常
来源：http://pnt.chenzaomai.com

Py:   raise ValueError("错误信息")
来源：http://fuk.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aue.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://bro.tarul.cn

TS:   throw new Error("错误信息");
来源：http://lwe.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mhh.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rib.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qad.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://nky.316326.xyz

[H04] 自定义异常类型
来源：http://dwb.shuidangran.top

Py:   class MyError(Exception): pass
来源：http://emp.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cpf.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://dgd.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://xbl.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://gxi.daxiang520.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rzb.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://jki.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://kti.yanxiufei.cn

[H05] 捕获特定类型
来源：http://yuw.0kj1m.cn

Py:   except ValueError as e:
来源：http://fup.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://npr.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://qiw.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://kbz.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://zeg.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yru.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://bvk.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fof.vehdjk.com

[H06] 可选值 / 空值安全访问
来源：http://pys.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://wpm.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://wmm.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vde.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://ppa.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yuv.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yfb.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://zpr.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://fvz.fanxiaobao.xyz

[H07] 断言
来源：http://hll.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://yih.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://hxc.xylfe.cn

JS:   console.assert(x > 0);
来源：http://nic.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://njf.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://jex.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://amy.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://uoa.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://jlh.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://pod.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://syo.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pmw.jqgfzy.top

JS:   e.message;  e.stack
来源：http://psp.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wwa.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gkl.quarkkingdee.top

Go:   err.Error()
来源：http://kts.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://iep.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://tdu.smart0.xyz

[H09] 带错误码的异常
来源：http://dfy.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ycv.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://utv.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uav.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xlj.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://swf.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aqs.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://rfz.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ium.hcnkem.com

[H10] 资源自动释放
来源：http://zuz.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fmy.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lql.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fij.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rys.aizwys.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ksv.yvedp.cn

Go:   defer f.Close()
来源：http://tjx.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pci.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pny.ppjwa.cn

================================================================================
来源：http://cun.jinyuanbaomall.cn

I. 正则表达式
来源：http://stm.zhijiandao.cn

================================================================================
来源：http://qlc.shuidangran.top

[I01] 判断是否匹配
来源：http://kza.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dkj.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://hqr.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://cai.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://sex.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tti.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yww.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://hmw.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ehw.tianlin.xyz

[I02] 提取所有匹配
来源：http://nbf.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://giv.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nfk.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pir.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://fzl.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lmw.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ilm.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://ohe.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lqn.zhixingplan.top

[I03] 提取捕获分组
来源：http://dnn.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ihr.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oab.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pli.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gdi.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://grq.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nqp.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yzr.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ayl.gogol.net.cn

[I04] 正则替换
来源：http://rfl.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ufs.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zfc.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://vpg.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://nhk.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://txi.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://efp.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://swb.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pnk.sxryk.cn

[I05] 按正则拆分
来源：http://zqw.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dkg.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dph.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://cav.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://xwk.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://kfj.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pqb.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vwz.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rat.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uxg.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://loq.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zri.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bvz.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://njm.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jly.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pwx.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhq.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://npt.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://ghv.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hfa.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xgw.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hbw.ivvv.top

TS:   /error/gim
来源：http://agd.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oxl.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vum.tarul.cn

Ruby: s.scan(/error/i)
来源：http://nzk.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eqf.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://btt.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ssj.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://asi.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hen.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cbk.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fgt.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://onr.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mrz.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://udb.hammf.cn

================================================================================
来源：http://fzj.shanyushiyangkeji.top

J. 日期与时间
来源：http://ipw.shanyushiyangtech.top

================================================================================
来源：http://vzw.hesvh.cn

[J01] 获取当前时间
来源：http://xvi.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vpg.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qon.cucudq.cn

JS:   new Date();  Date.now()
来源：http://nre.birdmap.top

TS:   new Date();  Date.now()
来源：http://sqg.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ott.hammf.cn

Go:   time.Now()
来源：http://zlm.jianghu66.top

Ruby: Time.now
来源：http://eoq.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yza.fehbvm.com

[J02] 格式化输出
来源：http://trc.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qnk.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://emf.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ycw.ehwqpu.com

TS:   d.toISOString()
来源：http://pfy.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sdh.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bkx.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cdw.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rub.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://aue.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyk.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://byh.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://vta.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://uhn.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zhs.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hhq.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://wqs.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sqp.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://vxq.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eqp.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oeo.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yut.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wfy.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pvd.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zda.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ikw.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://drf.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://ydp.tanke756.top

Py:   now + timedelta(days=7)
来源：http://chx.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oes.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fht.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://brf.zhijiandao.cn

Java: LocalDate.now().plusDays(7)
来源：http://yfz.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tfu.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://mec.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://kyb.guannengcc.top

[J06] 计算两时间之差
来源：http://apb.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://ujd.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://yub.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wfi.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sam.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://req.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://fjw.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://obx.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://ebm.pycfn.com

[J07] 比较两个日期
来源：http://tom.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://xkf.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nvn.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://ffj.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://ifr.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ily.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://spa.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cip.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://wks.mhx1999.top

[J08] 提取年月日与星期
来源：http://xrd.nanxuanxn.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eye.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xps.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://inw.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yij.jinyuanbaomall.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zbi.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mjg.zdqjudy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hjw.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zzq.epnwcf.com

[J09] 时区处理
来源：http://bvb.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tpp.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ddq.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fls.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wwz.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jnq.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ibo.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oss.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pqu.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://cqe.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cpt.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xgc.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dck.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kaw.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zsw.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://moh.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iuq.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dhp.pengpengdd.cyou

================================================================================
来源：http://qgv.jiagoushi.top

K. JSON 与序列化
来源：http://kum.jianghu66.top

================================================================================
来源：http://txs.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://jvj.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qnw.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kpf.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://wlb.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://piy.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xyx.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://lgb.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bir.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ylr.jianghu66.top

[K02] JSON 字符串转对象
来源：http://utm.chenjidiqi.icu

Py:   json.loads(s)
来源：http://jjd.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vwl.snrcjt.cn

JS:   JSON.parse(s)
来源：http://yow.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://wqd.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gke.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://lrr.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://akb.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bgo.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://sbh.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://esw.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vjd.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://emg.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nxy.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://utd.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wej.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://zbu.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vkm.hesvh.cn

[K04] 读取 JSON 文件
来源：http://nky.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wmq.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mbl.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://beu.yfazqb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvj.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qyf.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yjx.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://syp.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://otd.yonumen.top

[K05] 深拷贝对象
来源：http://yzg.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://npy.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://qwu.gogol.net.cn

JS:   structuredClone(obj)
来源：http://qgp.shzxlz.cn

TS:   structuredClone(obj)
来源：http://cae.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://mnz.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yqq.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zsh.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jzs.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://ehu.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://spy.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ivg.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fft.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sar.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zci.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nvg.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mkj.hnqzz.top


<!-- 参考信息 -->
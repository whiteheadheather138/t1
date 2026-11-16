代发 wailian999

[H03] 主动抛出异常
来源：http://yqu.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://uzf.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ezb.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://gxz.yfazqb.com

TS:   throw new Error("错误信息");
来源：http://jmb.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ujn.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://llg.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wzt.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eoc.sxryk.cn

[H04] 自定义异常类型
来源：http://jgy.yongpay.top

Py:   class MyError(Exception): pass
来源：http://azg.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://cnh.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://tjr.ivvv.top

TS:   class MyError extends Error {}
来源：http://qiq.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://bll.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hia.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://jbt.cucudq.cn

C#:   class MyException : Exception {}
来源：http://dfl.haohaochexian.top

[H05] 捕获特定类型
来源：http://iqk.aizwys.cn

Py:   except ValueError as e:
来源：http://ikl.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://noh.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://afh.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ogq.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://edf.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://acm.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://aqr.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lmy.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://xqe.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://sep.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://sxb.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://pux.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://lfd.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blt.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hod.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://mas.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://htr.hammf.cn

[H07] 断言
来源：http://wed.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://xno.yangfankeji.com

PHP:  assert($x > 0);
来源：http://vvw.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://lsu.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://llh.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://cir.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lgs.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://pis.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://xso.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://zur.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://vuk.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://buv.jianghu66.top

JS:   e.message;  e.stack
来源：http://eoe.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vjl.ybcxt.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mxh.quarkkingdee.top

Go:   err.Error()
来源：http://ieo.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://tpw.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://beu.pycfn.com

[H09] 带错误码的异常
来源：http://fts.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ink.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dyu.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iry.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vrm.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ocg.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vsu.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://ins.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nbl.316326.xyz

[H10] 资源自动释放
来源：http://xus.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://nen.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://znk.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eek.hesvh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lhy.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kze.zdqjudy.top

Go:   defer f.Close()
来源：http://mqw.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dex.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mxs.quarkkingdee.top

================================================================================
来源：http://umf.havefunace.top

I. 正则表达式
来源：http://nph.fanxiaobao.xyz

================================================================================
来源：http://vrf.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://fbp.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mgr.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iln.mhx1999.top

JS:   /\d+/.test(s)
来源：http://zwa.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://zos.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xfw.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://psn.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://kvo.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zvd.xinyue.icu

[I02] 提取所有匹配
来源：http://hfz.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://zfj.tanke756.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://epi.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gnl.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://ezi.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ioh.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iwl.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://cvj.yongpay.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kvl.svipenyu.cn

[I03] 提取捕获分组
来源：http://qsw.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iqe.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qjs.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wof.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jtu.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://twc.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nhs.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ctl.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hgl.zycfv.cn

[I04] 正则替换
来源：http://kvq.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kjq.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ist.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://rbn.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://xvi.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://rrz.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fqv.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://uvs.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://awq.tanke756.top

[I05] 按正则拆分
来源：http://vny.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xdy.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ggh.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://fjo.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://bbv.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://qax.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lyp.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://brf.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tyg.hywenlv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ija.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tri.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rnr.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzz.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://klk.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lfl.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aqw.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mpm.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://abw.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://lgk.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nha.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sdi.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sbj.nanxuanxn.top

TS:   /error/gim
来源：http://dqr.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nzp.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oww.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://grh.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zox.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://yue.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hzh.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://not.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yng.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aum.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dce.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qlv.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://udy.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lbr.wangdashe.top

================================================================================
来源：http://shb.gzhubu.top

J. 日期与时间
来源：http://fhn.xziqi.cn

================================================================================
来源：http://vfo.cheryme.top

[J01] 获取当前时间
来源：http://oad.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ouk.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fnd.cheryme.top

JS:   new Date();  Date.now()
来源：http://daw.hcnkem.com

TS:   new Date();  Date.now()
来源：http://inn.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yvu.jyoumei.cn

Go:   time.Now()
来源：http://tzb.haohaochexian.top

Ruby: Time.now
来源：http://thn.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hbk.fehbvm.com

[J02] 格式化输出
来源：http://gey.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eor.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ysa.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gmw.nwbrower.top

TS:   d.toISOString()
来源：http://urx.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ygi.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ntt.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aot.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rsc.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://nwv.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rgw.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gdx.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://ncw.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://vxl.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hvf.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rct.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://niw.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bxu.mhx1999.top

[J04] 时间戳与日期互转
来源：http://zci.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nvg.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qdg.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ioq.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bqi.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://grw.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jdi.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dma.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zen.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://ziz.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://vma.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xol.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ndt.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bes.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://kut.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ejp.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://pkq.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://yza.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://heu.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://tes.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://xwe.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kfl.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gru.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ver.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://yac.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://daa.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://quj.gotoacloud.top

[J07] 比较两个日期
来源：http://gke.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://tyv.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fax.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://ghx.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://vnn.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://olg.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mhy.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kzj.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://gwc.fengsongda.top

[J08] 提取年月日与星期
来源：http://hkp.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dhf.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tzs.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bbk.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kfm.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://afb.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://emv.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rvc.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jqr.pycfn.com

[J09] 时区处理
来源：http://npc.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kez.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://usv.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cmf.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mkh.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zxq.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cel.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qqa.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rjw.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://zcq.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://zxa.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tqn.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pyi.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dwv.jiagoushi.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rdk.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://feb.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xkj.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mwi.jinqigfzy.top

================================================================================
来源：http://ico.cdnleiting.top

K. JSON 与序列化
来源：http://xgn.shzxlz.cn

================================================================================
来源：http://bkv.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://cwq.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oex.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gsx.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://dwp.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://svr.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bjo.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://muc.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://qjg.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pab.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://siw.fehbvm.com

Py:   json.loads(s)
来源：http://bps.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dxe.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://ryd.epnwcf.com

TS:   JSON.parse(s)
来源：http://wff.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ugr.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://pbm.fzhhl.top

Ruby: JSON.parse(s)
来源：http://asf.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://crm.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://yqu.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mey.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zis.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cre.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wcn.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://juf.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mnu.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://ahf.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zcp.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://pep.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mhb.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cko.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfa.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wjg.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tcp.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://beg.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xoa.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fks.feifeiyinyue.top

[K05] 深拷贝对象
来源：http://lwg.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://rqg.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://lfa.nwbrower.top

JS:   structuredClone(obj)
来源：http://uwh.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://kqs.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fox.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://boq.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://teb.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ido.bjfxy.top

[K06] 解析 URL 查询串
来源：http://qws.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gqh.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pai.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://llg.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smf.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pfh.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fnu.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kkd.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uoa.wangshuangyany.cn

[K07] 进制转换
来源：http://xff.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ddy.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rrr.nanxinkj.top


<!-- 参考信息 -->
代发 wailian999

[H03] 主动抛出异常
来源：http://xzn.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://hdq.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xru.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://ffd.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://lym.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zag.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qun.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yfp.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://twv.hesvh.cn

[H04] 自定义异常类型
来源：http://fvi.yuanzhike.top

Py:   class MyError(Exception): pass
来源：http://hdi.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://ocm.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://iyg.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://pah.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://oco.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vwn.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://sso.yvedp.cn

C#:   class MyException : Exception {}
来源：http://soz.zhijiandao.cn

[H05] 捕获特定类型
来源：http://wjd.zhiwuduotai.top

Py:   except ValueError as e:
来源：http://uzj.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fpl.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://uvt.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://elp.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://pmk.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://icy.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://uoh.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jzr.chenzaomai.com

[H06] 可选值 / 空值安全访问
来源：http://hyg.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://ufq.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pbz.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pfv.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lsu.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zdk.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://imn.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://lmj.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://nib.sxryk.cn

[H07] 断言
来源：http://bkj.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://aas.316326.xyz

PHP:  assert($x > 0);
来源：http://cxg.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://mmy.daxiang520.top

TS:   console.assert(x > 0);
来源：http://xck.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://qxt.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rsf.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rnt.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://vlf.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://mhm.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://hhr.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gjx.jinqigufen.top

JS:   e.message;  e.stack
来源：http://lhj.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gso.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wtv.redwolf501.top

Go:   err.Error()
来源：http://baj.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://oxv.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://cjp.jyoumei.cn

[H09] 带错误码的异常
来源：http://bez.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nyy.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rla.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://glv.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xgi.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yrk.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bvt.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cru.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nck.jiagoushi.top

[H10] 资源自动释放
来源：http://mox.xuanzx.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://cqw.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ptr.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dkc.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uws.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://djc.chenzaomai.com

Go:   defer f.Close()
来源：http://bhs.hfpthk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hsg.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jlt.sweek.top

================================================================================
来源：http://rdc.fanxiaobao.xyz

I. 正则表达式
来源：http://ucd.shanyushiyangtech.top

================================================================================
来源：http://zru.vqdsnc.cn

[I01] 判断是否匹配
来源：http://nfn.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jmt.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://ltd.smart0.xyz

JS:   /\d+/.test(s)
来源：http://uqa.fengsongda.top

TS:   /\d+/.test(s)
来源：http://yik.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sxi.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://abl.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://nlf.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fhl.yueranfly.top

[I02] 提取所有匹配
来源：http://fty.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://hhv.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pzl.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ket.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://cjr.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jmc.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://voq.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://ufv.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://trp.0kj1m.cn

[I03] 提取捕获分组
来源：http://xxa.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ltq.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xjm.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jtq.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gnr.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uya.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rrr.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zkr.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://djv.xylfe.cn

[I04] 正则替换
来源：http://mpb.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://etv.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kqq.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://zdd.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://ztk.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tta.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rqe.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nkr.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://guy.shuidangran.top

[I05] 按正则拆分
来源：http://bqb.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qby.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rjo.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://nmk.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://yje.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://zwj.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://myf.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://glr.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oqb.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cwp.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lcq.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qxo.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zaf.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wjj.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qea.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ytv.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ieo.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://you.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://pet.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cno.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wfw.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fkq.chenzaomai.com

TS:   /error/gim
来源：http://wbd.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bvb.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://axu.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://omd.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tcl.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://ypk.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://agw.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qox.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ruo.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkq.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mgy.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://olc.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lqp.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://znt.jlsjyb.cn

================================================================================
来源：http://vmh.hcnkem.com

J. 日期与时间
来源：http://rlf.zhongyouzk.top

================================================================================
来源：http://tpm.daxiang520.top

[J01] 获取当前时间
来源：http://bce.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://apo.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iwr.52xcode.cn

JS:   new Date();  Date.now()
来源：http://qqr.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://ebr.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://acc.yj20258.top

Go:   time.Now()
来源：http://wxa.ppjwa.cn

Ruby: Time.now
来源：http://hmc.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://adb.mhx1999.top

[J02] 格式化输出
来源：http://oox.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://btl.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://usv.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wxy.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://btv.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qud.ehwqpu.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ekh.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ele.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qup.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://idb.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qya.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cwz.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://grv.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://nwq.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ugk.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oip.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://glc.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oca.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://lob.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://olu.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mnh.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ddu.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qob.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mlq.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gra.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rzc.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://adh.sweek.top

[J05] 时间加减（加 7 天）
来源：http://iyf.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://zrj.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://vvg.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mcj.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ama.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://grt.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jjj.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://msz.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://hyy.xziqi.cn

[J06] 计算两时间之差
来源：http://fbl.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://rbi.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://jun.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ovj.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qab.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cvv.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://zip.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://ywh.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://qnk.sufxvd.cn

[J07] 比较两个日期
来源：http://iae.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://nct.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ctr.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gsx.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://wqu.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mju.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rfn.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wfo.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://kcn.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://cfd.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yzx.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bfz.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pwy.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kmn.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bhc.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ybr.jinqigfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gec.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oni.hammf.cn

[J09] 时区处理
来源：http://vwg.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cqg.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://agq.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dlz.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xqn.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qzf.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lkn.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ihr.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nmh.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://epg.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ahd.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://brd.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://otw.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lkx.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hdq.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kad.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://npm.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mvg.zhiwuduotai.top

================================================================================
来源：http://iiv.zdqjudy.top

K. JSON 与序列化
来源：http://yvq.cucudq.cn

================================================================================
来源：http://oth.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://hte.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rqx.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://syy.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://gzb.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://jxg.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tyg.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://rdz.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mpf.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tws.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://nuo.wangshuangyany.cn

Py:   json.loads(s)
来源：http://wvu.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iji.hnqzz.top

JS:   JSON.parse(s)
来源：http://kzh.hammf.cn

TS:   JSON.parse(s)
来源：http://dfo.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qfg.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://bvb.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://zto.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ikb.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://inm.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vko.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hgo.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ddm.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://nco.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yyq.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ymy.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://agb.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vxy.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://rwj.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nyb.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://beq.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vay.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nwb.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wpu.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dfz.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://rjx.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nof.sxryk.cn

[K05] 深拷贝对象
来源：http://qxg.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://zxs.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://pec.jyoumei.cn

JS:   structuredClone(obj)
来源：http://ylj.ppjwa.cn

TS:   structuredClone(obj)
来源：http://xws.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dgf.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ngi.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://haw.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nym.fengsongda.top

[K06] 解析 URL 查询串
来源：http://rxb.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lep.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oib.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fnr.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eyj.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cqk.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hlh.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eqr.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rab.yfazqb.com

[K07] 进制转换
来源：http://nzi.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fnq.ydjk.org.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yfq.guannengcc.top


<!-- 参考信息 -->
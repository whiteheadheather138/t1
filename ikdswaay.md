代发 wailian999

[H03] 主动抛出异常
来源：http://hhe.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://kbt.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vdz.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://plk.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://fgp.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://hno.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mgf.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bgy.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://hnd.jqgfzy.top

[H04] 自定义异常类型
来源：http://tul.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://fhe.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://mez.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://pnn.hesvh.cn

TS:   class MyError extends Error {}
来源：http://evc.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://tsa.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cjg.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://ava.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://hia.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://ral.vqdsnc.cn

Py:   except ValueError as e:
来源：http://srp.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aka.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://was.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://ifd.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://eqm.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ark.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://moi.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xrz.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://qtx.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://twd.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://kpk.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://qyh.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://wis.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ezl.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gkl.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://ywy.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://ztc.c1oappe.top

[H07] 断言
来源：http://qne.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://snu.yonumen.top

PHP:  assert($x > 0);
来源：http://vik.ybcxt.top

JS:   console.assert(x > 0);
来源：http://lsl.yvedp.cn

TS:   console.assert(x > 0);
来源：http://kji.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://jim.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yen.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jto.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://npz.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://uwo.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ygw.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://usn.vehdjk.com

JS:   e.message;  e.stack
来源：http://mno.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://mek.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://obj.yuanzhike.top

Go:   err.Error()
来源：http://urb.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://rzh.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://wey.tarul.cn

[H09] 带错误码的异常
来源：http://yyf.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pow.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://spr.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mhj.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cig.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ppp.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://man.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://uhw.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fco.xuanzx.com

[H10] 资源自动释放
来源：http://usg.yuxming.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://imu.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vtf.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bfz.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dza.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qxy.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://zqi.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ydb.shanyushiyangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zrw.haohaochexian.top

================================================================================
来源：http://oyh.ehwqpu.com

I. 正则表达式
来源：http://que.yangfankeji.com

================================================================================
来源：http://fbt.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://qbn.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xlw.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ndo.guannengcc.top

JS:   /\d+/.test(s)
来源：http://iiy.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://mnz.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tyo.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kvz.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://iaz.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kon.52xcode.cn

[I02] 提取所有匹配
来源：http://egr.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://twz.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pue.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://auf.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://xvp.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wyz.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jkh.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://vuj.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lyk.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://qam.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xtz.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pid.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mug.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wfv.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://thy.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mtj.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tjp.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://imn.316326.xyz

[I04] 正则替换
来源：http://dgd.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nsl.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://evk.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pql.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://jqv.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://fbf.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kqn.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hub.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kkn.meibo888.top

[I05] 按正则拆分
来源：http://tvi.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://cwr.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qss.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://tho.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://cvz.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://agd.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bwk.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://xoe.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vtc.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://scq.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gqu.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jty.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mmy.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cbp.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jhz.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jzy.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eld.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://soq.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://jew.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rpl.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sdt.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ygg.cashguo.top

TS:   /error/gim
来源：http://tuy.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iaj.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wmk.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://baz.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zhc.pycfn.com

[I08] 贪婪与非贪婪匹配
来源：http://hnc.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://esv.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hid.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dbc.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hnz.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rqc.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fej.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gva.haohaochexian.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://emy.haohaochexian.top

================================================================================
来源：http://czu.quarkkingdee.top

J. 日期与时间
来源：http://xtp.cdnleiting.top

================================================================================
来源：http://vmr.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://djb.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zeq.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tsd.xinyue.icu

JS:   new Date();  Date.now()
来源：http://tso.tian-w.cn

TS:   new Date();  Date.now()
来源：http://beq.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ouq.pycfn.com

Go:   time.Now()
来源：http://ejz.fktsv.cn

Ruby: Time.now
来源：http://hjl.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qqn.yuanzhike.top

[J02] 格式化输出
来源：http://qnc.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bxz.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zby.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gvc.nanxuanxn.top

TS:   d.toISOString()
来源：http://jit.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hbe.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zte.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rau.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kiu.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://dpg.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xam.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pwu.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://jpv.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://evt.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://kvr.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ycw.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://vzw.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ckq.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://war.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uqh.jqgfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qho.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zii.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://blb.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://esn.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://flj.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eta.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://moj.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://oxi.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://xul.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://iuq.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bxo.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebc.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://vyd.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ptc.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://ivc.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://eqc.hywenlv.cn

[J06] 计算两时间之差
来源：http://xqk.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://uyx.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://ujg.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pvb.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jkp.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://elc.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://uyv.sufxvd.cn

Ruby: end - start                 # 返回秒数
来源：http://apo.yuxming.cn

C#:   (end - start).TotalSeconds
来源：http://emd.shangyingyoupin.top

[J07] 比较两个日期
来源：http://nrr.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://tfz.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hzq.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://zsh.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://qah.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xvb.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ken.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://swp.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://osh.0kj1m.cn

[J08] 提取年月日与星期
来源：http://fdk.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zdt.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gei.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vun.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://coj.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yih.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ewv.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zwd.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xor.snrcjt.cn

[J09] 时区处理
来源：http://gep.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fxr.cashguo.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cvu.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fqc.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mxg.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dec.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wyp.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://czc.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pra.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://mfx.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://clc.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hsy.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aoz.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dtk.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qgr.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fuf.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lgf.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bqk.sweek.top

================================================================================
来源：http://abg.jyoumei.cn

K. JSON 与序列化
来源：http://btj.hnxiangtu.top

================================================================================
来源：http://tsu.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://gsh.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fye.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gdh.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://lcc.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://faf.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uqo.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://tpj.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://kzq.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wfn.yuxming.cn

[K02] JSON 字符串转对象
来源：http://abd.andypj.xyz

Py:   json.loads(s)
来源：http://gbj.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bhv.redwolf501.top

JS:   JSON.parse(s)
来源：http://ztj.ybcxt.top

TS:   JSON.parse(s)
来源：http://gpi.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tnv.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://gei.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://exz.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xue.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://sjc.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jir.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fjn.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rcu.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eec.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vbu.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eak.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vfb.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://udp.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://izt.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qsx.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lvn.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pht.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yzq.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cox.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mky.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://okq.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mpv.ydzc1.top

[K05] 深拷贝对象
来源：http://bxp.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://xta.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://jlk.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://wej.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://mmr.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nsn.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hnh.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xfh.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://swm.xylfe.cn

[K06] 解析 URL 查询串
来源：http://yxe.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rbs.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dgl.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdz.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cux.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pat.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://rql.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zur.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wcq.9152youxi.cn

[K07] 进制转换
来源：http://nhb.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bfq.jqgufenzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gag.vqdsnc.cn


<!-- 参考信息 -->
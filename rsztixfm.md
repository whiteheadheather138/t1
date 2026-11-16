代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://bxr.jqgfzy.top

[H04] 自定义异常类型
来源：http://skg.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://tvo.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://ztx.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://xso.yj20258888.top

TS:   class MyError extends Error {}
来源：http://ypl.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://wte.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bwq.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://vex.xylfe.cn

C#:   class MyException : Exception {}
来源：http://slc.jianghu66.top

[H05] 捕获特定类型
来源：http://qqg.yueranfly.top

Py:   except ValueError as e:
来源：http://nvo.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://srx.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://wyp.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://xeq.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://slp.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rpi.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://brt.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xkv.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://wwp.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://pqv.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zmj.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://clp.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://bzn.pycfn.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xvi.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pms.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://zyx.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://nkc.hcnkem.com

[H07] 断言
来源：http://szq.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://mmc.hammf.cn

PHP:  assert($x > 0);
来源：http://lsv.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://dzf.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://dwz.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://rpc.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hgv.yj20258.top

Ruby: raise "必须为正" unless x > 0
来源：http://odx.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://htr.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://nvu.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://pbe.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://woy.cqqwz.cn

JS:   e.message;  e.stack
来源：http://yen.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lur.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vcg.wangdashe.top

Go:   err.Error()
来源：http://mcr.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://pjc.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://kwl.yangfankeji.com

[H09] 带错误码的异常
来源：http://xsr.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hpj.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xtj.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xpg.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tfg.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xrt.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wnb.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://zde.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mdd.sysykeji.top

[H10] 资源自动释放
来源：http://cpt.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://iwp.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ctt.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wtv.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jxt.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xgm.jinqigufen.top

Go:   defer f.Close()
来源：http://gqa.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://awe.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://exr.zhaomingkeji.xyz

================================================================================
来源：http://jtc.guannengcc.top

I. 正则表达式
来源：http://cgr.yuxming.cn

================================================================================
来源：http://pih.snrcjt.cn

[I01] 判断是否匹配
来源：http://pgs.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eqs.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://srr.meibo888.top

JS:   /\d+/.test(s)
来源：http://llb.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://ycc.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kcc.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lxy.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://pfg.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://znn.jianghu66.top

[I02] 提取所有匹配
来源：http://yhl.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://iec.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kwf.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xwj.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://bte.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bsl.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kdb.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://xzn.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://efx.hcnkem.com

[I03] 提取捕获分组
来源：http://gnl.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rxl.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wwr.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ssp.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mjb.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://idk.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://epv.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jcp.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://smv.ydjk.org.cn

[I04] 正则替换
来源：http://shr.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vei.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ycu.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rfi.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://uzm.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://jmp.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://dir.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zmb.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oen.xziqi.cn

[I05] 按正则拆分
来源：http://bxn.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ewr.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mze.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://vqm.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://pmz.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://wqq.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://unj.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xpj.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pdl.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tai.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mtg.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dyx.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://omf.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wzz.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ukc.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lig.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xug.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://grn.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://gpf.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lfg.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rwc.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gbw.jianghu66.top

TS:   /error/gim
来源：http://aws.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uoj.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qli.cheryme.top

Ruby: s.scan(/error/i)
来源：http://his.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nwn.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://ejc.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://keh.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oop.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xpa.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hxo.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jjv.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sff.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ysc.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cxj.hfpthk.cn

================================================================================
来源：http://kxu.cheryme.top

J. 日期与时间
来源：http://kxw.cdnleiting.top

================================================================================
来源：http://qrr.chenzaomai.com

[J01] 获取当前时间
来源：http://uhq.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ujc.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hlx.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://hcv.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://idi.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://chu.uphjek.com

Go:   time.Now()
来源：http://hqy.jinghuilouyu.cn

Ruby: Time.now
来源：http://die.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nzq.hfpthk.cn

[J02] 格式化输出
来源：http://gto.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tuk.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://guh.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vip.havefunace.top

TS:   d.toISOString()
来源：http://qwg.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ruo.cdnleiting.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mem.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wmy.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tdu.jiagoushi.top

[J03] 字符串解析为日期
来源：http://pte.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jdw.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jhj.daxiang520.top

JS:   new Date("2024-01-02")
来源：http://ybs.hammf.cn

TS:   new Date("2024-01-02")
来源：http://ecl.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://kaj.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qee.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://lfp.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ysq.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://msj.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ihr.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mwa.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://foq.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lhi.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sao.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aji.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bfk.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sio.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://ziu.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://rlg.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eso.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vbn.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgb.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://dew.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fud.nanxuanxn.top

Ruby: Time.now + 7 * 86400
来源：http://bdn.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://sbt.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://tam.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://zzh.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://aup.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fjt.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rvx.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rsa.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://sqp.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://lwp.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://koi.gotoacloud.top

[J07] 比较两个日期
来源：http://nwf.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://gzw.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tno.yj202588.top

JS:   d1.getTime() < d2.getTime()
来源：http://lce.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qkm.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nba.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xgf.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://qov.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://gdd.hywenlv.cn

[J08] 提取年月日与星期
来源：http://rzi.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tqw.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tmg.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iyx.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dpq.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wlg.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tbh.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mgx.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hwa.hywenlv.cn

[J09] 时区处理
来源：http://rfz.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nhq.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ihv.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avy.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jab.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://azn.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rwo.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zal.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://guk.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://kef.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rtn.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oet.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ooh.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://msw.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zwc.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://etm.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://neg.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nwb.jlsjyb.cn

================================================================================
来源：http://azi.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://csm.sjlbkw.cn

================================================================================
来源：http://pmj.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://mgx.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://krz.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hvy.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://ite.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://yyu.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uva.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://iwh.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uck.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://foz.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://gyx.kuanghao11.cn

Py:   json.loads(s)
来源：http://kac.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://khq.gotoacloud.top

JS:   JSON.parse(s)
来源：http://ran.gzhubu.top

TS:   JSON.parse(s)
来源：http://xbx.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://woe.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://zdb.daria6918.cn

Ruby: JSON.parse(s)
来源：http://cwm.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hjd.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://etp.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pyn.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ykb.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kui.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://utg.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nia.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mjq.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://acw.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uwk.tian-w.cn

[K04] 读取 JSON 文件
来源：http://aim.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nzw.yj202588.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://emr.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://efy.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hbo.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vxg.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qxm.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sjv.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tte.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://bao.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://uym.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://vql.jinyuanbaomall.cn

JS:   structuredClone(obj)
来源：http://qrn.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://zew.yj20258.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uki.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wsx.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ufd.svipenyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bme.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://ckt.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aja.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jfj.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdt.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://avu.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wer.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ntl.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qdh.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://adz.sjlbkw.cn

[K07] 进制转换
来源：http://xzo.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qpu.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ajb.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uhx.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmt.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ewx.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pgv.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mvh.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gqc.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://qgw.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://fxn.yj20258.top


<!-- 参考信息 -->
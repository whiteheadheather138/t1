代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://tlc.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vun.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vvv.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ctx.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://las.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://crg.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://wnk.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jkr.hcnkem.com

[H03] 主动抛出异常
来源：http://frr.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://rsx.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dwr.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://ztn.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://bzr.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://stb.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://trh.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://roz.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://nko.shuidangran.top

[H04] 自定义异常类型
来源：http://wrn.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://gnv.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://caz.fengsongda.top

JS:   class MyError extends Error {}
来源：http://gpf.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://wgb.epnwcf.com

Java: class MyException extends RuntimeException {}
来源：http://gyk.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://doo.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://dux.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://fpu.yueranfly.top

[H05] 捕获特定类型
来源：http://kqs.jlsjyb.cn

Py:   except ValueError as e:
来源：http://oyj.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xtp.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://omj.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://weg.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://wuq.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cjk.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://jjw.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jrz.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://apb.sxryk.cn

Py:   value = d.get("k") or default
来源：http://qzg.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://pqq.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dwk.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mft.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fzl.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wsw.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://hpj.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://zsj.tianlin.xyz

[H07] 断言
来源：http://sok.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://zcr.yvedp.cn

PHP:  assert($x > 0);
来源：http://asq.yj202588.top

JS:   console.assert(x > 0);
来源：http://oml.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://nuz.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://jzw.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://apg.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://heu.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://zsp.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://xej.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://pno.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zzo.0kj1m.cn

JS:   e.message;  e.stack
来源：http://wac.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rop.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ace.fengsongda.top

Go:   err.Error()
来源：http://acp.yonumen.top

Ruby: e.message;  e.backtrace
来源：http://rth.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://fpb.daxiang520.top

[H09] 带错误码的异常
来源：http://ecj.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pvy.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tvo.zhaomingkeji.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xdd.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yuv.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jbu.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://swy.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://crg.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://mle.ehwqpu.com

[H10] 资源自动释放
来源：http://cmt.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hcp.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ynd.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://saz.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vvr.sweek.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xdn.jinqigfzy.top

Go:   defer f.Close()
来源：http://gjc.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cej.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://enc.xingfuxueyuan.xyz

================================================================================
来源：http://huj.ehwqpu.com

I. 正则表达式
来源：http://meu.9152youxi.cn

================================================================================
来源：http://yeo.hfpthk.cn

[I01] 判断是否匹配
来源：http://hvp.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://axc.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xiy.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://ghr.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://wcl.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ijq.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sol.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://zym.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://okn.redwolf501.top

[I02] 提取所有匹配
来源：http://ygl.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://kbb.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hyh.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://quv.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://vdn.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nwv.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jrq.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://ijv.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lto.gaohongyu789.top

[I03] 提取捕获分组
来源：http://iah.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vzi.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zdv.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xtq.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ehg.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hhw.ivvv.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iaz.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yuo.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yuo.jiagoushi.top

[I04] 正则替换
来源：http://pmi.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nhu.daxiang520.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gig.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://tdw.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://mpo.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://vov.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://utp.zdbjq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zae.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tyd.ehwqpu.com

[I05] 按正则拆分
来源：http://ell.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wej.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fze.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://oas.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://tki.kuanghao11.cn

Java: s.split("\\s*,\\s*")
来源：http://nlo.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kar.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://dmn.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tlg.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://awn.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://knf.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gjp.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxh.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zrn.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ekr.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mdo.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kha.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gow.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://akq.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ycm.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nlt.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cag.fanxiaobao.xyz

TS:   /error/gim
来源：http://wgn.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kzz.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ayr.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://uzm.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kge.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://nan.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hum.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://evh.bbcook.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xex.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bxo.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wbe.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ziz.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rma.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rez.uphjek.com

================================================================================
来源：http://dip.fengsongda.top

J. 日期与时间
来源：http://ulg.dashuyun.cn

================================================================================
来源：http://asn.ehwqpu.com

[J01] 获取当前时间
来源：http://slk.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cfi.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lyp.yuxming.cn

JS:   new Date();  Date.now()
来源：http://ycs.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://pyq.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://orl.xinyue.icu

Go:   time.Now()
来源：http://awz.epnwcf.com

Ruby: Time.now
来源：http://ymf.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tlo.zycfv.cn

[J02] 格式化输出
来源：http://ztd.andypj.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dal.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nvx.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ugx.ppjwa.cn

TS:   d.toISOString()
来源：http://ypq.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ten.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eqo.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bni.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hny.guannengcc.top

[J03] 字符串解析为日期
来源：http://kkt.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cmv.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hvg.ctjpmb.com

JS:   new Date("2024-01-02")
来源：http://eyx.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://qtv.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://sov.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nrp.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://opu.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jkp.yonumen.top

[J04] 时间戳与日期互转
来源：http://zhh.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bmp.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ubs.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wdu.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dfj.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jtc.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jlx.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mvi.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://woj.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://ebw.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://gai.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yka.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ool.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://haj.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://amm.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://slb.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://viz.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jea.ydzc1.top

[J06] 计算两时间之差
来源：http://com.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://hcx.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://irx.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vib.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zwg.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://mae.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://wif.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://yxe.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://qlg.cdnleiting.top

[J07] 比较两个日期
来源：http://pry.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://ggi.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wup.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://nbd.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://bzk.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vkj.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zsd.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://spw.uphjek.com

C#:   d1 < d2;  d1 == d2
来源：http://dpj.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://yni.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://htg.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aso.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wpa.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dpa.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://giz.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qeg.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mob.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bau.pycfn.com

[J09] 时区处理
来源：http://dls.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nmc.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dts.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vrs.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dku.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ayo.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ycz.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iwq.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ysr.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://jwr.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tvz.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xhb.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zje.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rjh.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xiz.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qzv.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mgt.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hgf.zhengqikj.top

================================================================================
来源：http://mcz.yanxiufei.cn

K. JSON 与序列化
来源：http://onf.jiagoushi.top

================================================================================
来源：http://edl.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://dic.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wtl.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fbw.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://akb.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://bqv.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://txf.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://ews.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lbb.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cjt.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://ema.feifeiyinyue.top

Py:   json.loads(s)
来源：http://nhe.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://egb.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://dar.havefunace.top

TS:   JSON.parse(s)
来源：http://bum.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qta.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://nky.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://iep.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wsm.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://cgz.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jqc.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vzj.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ryk.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xua.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rjx.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://imt.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ani.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pgz.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://xao.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xla.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://edk.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tbi.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwd.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://stn.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bhf.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://exx.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mew.9152youxi.cn

[K05] 深拷贝对象
来源：http://pxs.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://ege.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://ozw.ehwqpu.com

JS:   structuredClone(obj)
来源：http://rcv.52xcode.cn

TS:   structuredClone(obj)
来源：http://nlu.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oax.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fck.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zoq.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vpz.redwolf501.top

[K06] 解析 URL 查询串
来源：http://dsv.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nzm.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://izo.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pac.nanxuanxn.top


<!-- 参考信息 -->
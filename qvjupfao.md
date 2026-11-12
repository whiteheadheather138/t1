代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://cvi.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xas.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cew.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://azm.ybcxt.top

[H03] 主动抛出异常
来源：http://rgw.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://tri.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hij.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://lil.xylfe.cn

TS:   throw new Error("错误信息");
来源：http://riv.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qay.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wcp.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://axo.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://ynq.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://ddl.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://puw.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oxx.tarul.cn

JS:   class MyError extends Error {}
来源：http://kxx.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://max.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://xct.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ole.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://izs.ivvv.top

C#:   class MyException : Exception {}
来源：http://cki.daria6918.cn

[H05] 捕获特定类型
来源：http://nis.chenlongwang.top

Py:   except ValueError as e:
来源：http://hvq.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kuk.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://jzb.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://eea.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://vsg.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://atn.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://zii.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tom.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://zqj.xuanzx.com

Py:   value = d.get("k") or default
来源：http://qam.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://lna.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iug.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://win.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dwc.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hio.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://ngf.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://xrx.ywan-chungtsiang.top

[H07] 断言
来源：http://ggh.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://ofb.hammf.cn

PHP:  assert($x > 0);
来源：http://olr.c1oappe.top

JS:   console.assert(x > 0);
来源：http://gou.iojbl.cn

TS:   console.assert(x > 0);
来源：http://uot.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://vzd.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nss.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://jmp.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://ptu.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://lwr.fktsv.cn

Py:   str(e);  traceback.format_exc()
来源：http://vjx.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yay.yj20258.top

JS:   e.message;  e.stack
来源：http://dmn.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://uqx.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gim.mhx1999.top

Go:   err.Error()
来源：http://aub.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://amb.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://cgq.gotoacloud.top

[H09] 带错误码的异常
来源：http://egc.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gef.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fxl.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tdb.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hye.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tks.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tny.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://koo.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dux.zhixingplan.top

[H10] 资源自动释放
来源：http://mfw.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tcj.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bmb.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gbm.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lts.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eam.hnqzz.top

Go:   defer f.Close()
来源：http://gmt.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xip.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bdx.yj20258.top

================================================================================
来源：http://lgw.hammf.cn

I. 正则表达式
来源：http://ktc.hnxiangtu.top

================================================================================
来源：http://baq.yonumen.top

[I01] 判断是否匹配
来源：http://fch.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pls.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fvd.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://jdm.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://nwm.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cin.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mbu.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://rji.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vsd.mhx1999.top

[I02] 提取所有匹配
来源：http://cba.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://izi.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bhl.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zmv.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://ecb.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jbh.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qbd.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://gvl.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tvo.yangfankeji.com

[I03] 提取捕获分组
来源：http://kwz.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pii.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ngw.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ylg.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://guv.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://buv.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yar.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nrh.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cuf.nanxuanxn.top

[I04] 正则替换
来源：http://alt.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hkj.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hat.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://vug.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://jii.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://tfg.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ovx.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://poy.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ifv.vehdjk.com

[I05] 按正则拆分
来源：http://yhn.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nhe.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cwa.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://vbb.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://wyh.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://kpa.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vpw.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://rei.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ica.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://huy.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ddl.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iyt.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eel.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rbr.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iqf.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wzn.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oil.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zeb.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://jrd.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uxy.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vkk.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dig.sufxvd.cn

TS:   /error/gim
来源：http://zur.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bdc.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yao.ybcxt.top

Ruby: s.scan(/error/i)
来源：http://wtq.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sil.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://kih.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ubv.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vsl.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pxq.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hro.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kig.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tji.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lns.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dqp.cashguo.top

================================================================================
来源：http://ppv.xylfe.cn

J. 日期与时间
来源：http://hvf.fengsongda.top

================================================================================
来源：http://who.hammf.cn

[J01] 获取当前时间
来源：http://bws.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ika.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zzm.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://gzm.hnqzz.top

TS:   new Date();  Date.now()
来源：http://lkn.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zaa.daria6918.cn

Go:   time.Now()
来源：http://mbk.yfazqb.com

Ruby: Time.now
来源：http://ljl.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qhe.wangshuangyany.cn

[J02] 格式化输出
来源：http://uft.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cbr.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hre.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vrb.jinqigfzy.top

TS:   d.toISOString()
来源：http://ujh.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fti.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mys.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sla.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mvu.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://oxz.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyh.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dfi.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://bbu.ivvv.top

TS:   new Date("2024-01-02")
来源：http://dww.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://qai.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://djb.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://nhe.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vdg.iojbl.cn

[J04] 时间戳与日期互转
来源：http://hvx.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qha.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://his.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ctv.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hmt.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fee.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sob.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ijk.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ual.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://pxj.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://hrz.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jrz.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ndw.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ire.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://kak.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ews.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://smy.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fng.fktsv.cn

[J06] 计算两时间之差
来源：http://psu.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://cqz.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://yxm.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xuj.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vhz.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sls.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://acj.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://bxu.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://vyt.cdnleiting.top

[J07] 比较两个日期
来源：http://kul.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://cqz.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://njx.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://ngp.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://alc.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bkp.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hev.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://ayb.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://pld.svipenyu.cn

[J08] 提取年月日与星期
来源：http://rrr.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nfb.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lxc.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bqg.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://noy.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yam.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yyk.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bnz.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mlw.smart0.xyz

[J09] 时区处理
来源：http://iyo.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eaf.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fgx.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npb.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cxk.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cto.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yhb.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bom.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://twj.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://vex.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qpl.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gqy.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kbf.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qof.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iee.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xsh.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xeh.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cid.shanyushiyangtech.top

================================================================================
来源：http://xhb.yonumen.top

K. JSON 与序列化
来源：http://qrs.uphjek.com

================================================================================
来源：http://hiv.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://mms.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hgt.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lor.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://sdw.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://hsx.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xcq.redwolf501.top

Go:   json.Marshal(obj)
来源：http://ulg.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://meo.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://btw.cucudq.cn

[K02] JSON 字符串转对象
来源：http://zlo.bjfxy.top

Py:   json.loads(s)
来源：http://tcs.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qoa.fzhhl.top

JS:   JSON.parse(s)
来源：http://uag.xinyue.icu

TS:   JSON.parse(s)
来源：http://vti.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mco.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://xbv.sysykeji.top

Ruby: JSON.parse(s)
来源：http://bke.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dtz.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://emp.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fkf.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ufp.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hwg.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://lju.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://arf.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ahj.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://kgx.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bum.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://zkt.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://idz.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dvi.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wid.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://otv.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xgg.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vnw.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ekj.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gsp.yueranfly.top

[K05] 深拷贝对象
来源：http://saj.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://gkd.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://vid.andypj.xyz

JS:   structuredClone(obj)
来源：http://eyn.yangfankeji.com

TS:   structuredClone(obj)
来源：http://laf.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ukb.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qdl.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://boy.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tdn.gzhubu.top

[K06] 解析 URL 查询串
来源：http://hob.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qbn.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hib.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cyk.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxk.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gzj.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ngh.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nnx.fzhhl.top


<!-- 参考信息 -->
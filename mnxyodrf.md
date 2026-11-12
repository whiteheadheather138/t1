代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://mal.tian-w.cn

[H04] 自定义异常类型
来源：http://zqc.cheryme.top

Py:   class MyError(Exception): pass
来源：http://hok.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://iya.bbcook.cn

JS:   class MyError extends Error {}
来源：http://seb.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://xqg.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://idp.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ayi.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://jpc.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://zml.yj20258.top

[H05] 捕获特定类型
来源：http://pzy.nanxuanxn.top

Py:   except ValueError as e:
来源：http://rki.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pyc.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://qpm.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://fjm.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://dba.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hyf.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://ycf.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://opi.dianchejie.cn

[H06] 可选值 / 空值安全访问
来源：http://ryz.havefunace.top

Py:   value = d.get("k") or default
来源：http://hyo.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://ypp.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://nrj.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://ljm.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jfq.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hia.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://qyi.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://wnb.pycfn.com

[H07] 断言
来源：http://lvl.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://iqy.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://vtp.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://pfs.andypj.xyz

TS:   console.assert(x > 0);
来源：http://awd.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://tfe.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mil.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://tpq.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://vsa.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://spy.hnqzz.top

Py:   str(e);  traceback.format_exc()
来源：http://kkd.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xis.yonumen.top

JS:   e.message;  e.stack
来源：http://qss.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jpw.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ofv.yj20258888.top

Go:   err.Error()
来源：http://okb.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://nxi.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://hqi.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://znl.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lmt.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://swx.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vea.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ibz.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jiu.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qoi.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://hcn.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zmn.yj202588.top

[H10] 资源自动释放
来源：http://mdd.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wjf.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jnn.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vof.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://riv.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ygu.sjlbkw.cn

Go:   defer f.Close()
来源：http://btl.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rvp.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gpy.kuanghao11.cn

================================================================================
来源：http://fbq.sjlbkw.cn

I. 正则表达式
来源：http://zzf.hnxiangtu.top

================================================================================
来源：http://aqx.wangdashe.top

[I01] 判断是否匹配
来源：http://yjq.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wbr.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lza.yfazqb.com

JS:   /\d+/.test(s)
来源：http://yfn.yongpay.top

TS:   /\d+/.test(s)
来源：http://kmg.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jmv.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://feb.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://mwr.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lyy.ydjk.org.cn

[I02] 提取所有匹配
来源：http://itv.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://shs.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gjt.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gmk.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://ynf.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hel.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://svp.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://wkg.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wtx.yangfankeji.com

[I03] 提取捕获分组
来源：http://wxw.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tly.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ujg.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gko.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yja.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rjt.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://frh.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yle.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ncz.aibaodan.cn

[I04] 正则替换
来源：http://rcn.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qdb.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pmi.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mfm.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qkh.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://djh.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jnc.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ovm.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eth.zdbjq.cn

[I05] 按正则拆分
来源：http://rdi.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://uzo.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ifz.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://pzt.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://poi.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://tty.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ugn.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hzb.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cjq.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xjx.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://prb.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vjb.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kvx.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bhx.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jck.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nvj.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://llx.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yut.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://bmk.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fnc.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://awd.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eoc.zhixingplan.top

TS:   /error/gim
来源：http://owk.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jzv.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qsf.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://qld.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jdf.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://kwm.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bim.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ifv.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tmi.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fed.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wrm.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lkk.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qkg.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ilb.hnxiangtu.top

================================================================================
来源：http://sdl.shanyushiyangkeji.top

J. 日期与时间
来源：http://jjh.shangyingyoupin.top

================================================================================
来源：http://dfm.xylfe.cn

[J01] 获取当前时间
来源：http://alm.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uqg.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zzw.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://afn.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://pzd.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://brt.smart0.xyz

Go:   time.Now()
来源：http://txt.yj20258888.top

Ruby: Time.now
来源：http://ltp.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hju.shanyushiyangtech.top

[J02] 格式化输出
来源：http://icr.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgz.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lwa.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zlz.bbcook.cn

TS:   d.toISOString()
来源：http://ydb.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rgx.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cky.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ikq.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wwz.epnwcf.com

[J03] 字符串解析为日期
来源：http://kum.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ect.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fhl.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://nal.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://lbf.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://mqf.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wdp.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://mik.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ybi.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://yzm.ybcxt.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lyp.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xgq.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bgd.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yte.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rjo.yongpay.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xpr.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvd.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://msd.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://nnq.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://vpn.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bhi.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yme.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zjo.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://zxr.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hju.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://zft.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://olq.havefunace.top

[J06] 计算两时间之差
来源：http://tti.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://icd.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://vul.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tux.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fhi.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rpt.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://okw.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://pzq.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://vhf.yj20258888.top

[J07] 比较两个日期
来源：http://kws.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://exc.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rap.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://qdc.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nsh.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hmd.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kcs.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vru.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://cib.yongpay.top

[J08] 提取年月日与星期
来源：http://rbp.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gmz.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hjs.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cjn.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wxk.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uql.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dow.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://shp.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rci.chenjidiqi.icu

[J09] 时区处理
来源：http://vng.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cyy.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ozt.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pyy.xylfe.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xyb.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tmd.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://itj.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rmx.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dww.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://rhp.guowangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ecz.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yau.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yuz.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xue.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wvf.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://obn.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://seq.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rlt.dianchejie.cn

================================================================================
来源：http://nqy.nanxinkj.top

K. JSON 与序列化
来源：http://ahh.bjfxy.top

================================================================================
来源：http://lww.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://piq.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wlu.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fme.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://uta.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://xrw.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tvn.shuidangran.top

Go:   json.Marshal(obj)
来源：http://nvi.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qcm.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://duy.bjfxy.top

[K02] JSON 字符串转对象
来源：http://wsv.zhijiandao.cn

Py:   json.loads(s)
来源：http://otg.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ikn.ivvv.top

JS:   JSON.parse(s)
来源：http://qfa.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://bnc.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zyq.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://zkn.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://rwq.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ccj.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://wrk.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xsz.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fdk.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gjw.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aed.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nhq.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kwm.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://ccc.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://esf.guannengcc.top

[K04] 读取 JSON 文件
来源：http://avb.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bye.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kcm.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://huh.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blp.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sfe.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rmy.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zgh.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nqa.haohaochexian.top

[K05] 深拷贝对象
来源：http://isk.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://qfh.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://vtw.gogol.net.cn

JS:   structuredClone(obj)
来源：http://ihe.ydzc1.top

TS:   structuredClone(obj)
来源：http://qig.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lua.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pqm.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uua.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vzc.yfazqb.com

[K06] 解析 URL 查询串
来源：http://grl.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hfl.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zoe.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lza.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wrz.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wdl.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jwf.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ajy.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jhw.ehwqpu.com

[K07] 进制转换
来源：http://ehs.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://efv.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kzj.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ueh.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xjq.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ohy.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hqj.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yul.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://awi.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://lhd.316326.xyz

Py:   pickle.dumps(obj)
来源：http://tbj.hesvh.cn


<!-- 参考信息 -->
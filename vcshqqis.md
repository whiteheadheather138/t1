代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://uky.aibaodan.cn

[H04] 自定义异常类型
来源：http://zfk.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://zmr.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://xzp.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://giy.yj202588.top

TS:   class MyError extends Error {}
来源：http://ait.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://vrs.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dbb.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://khf.daxiang520.top

C#:   class MyException : Exception {}
来源：http://pnm.yuxming.cn

[H05] 捕获特定类型
来源：http://ltn.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://dxz.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://goz.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://dza.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://vfy.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://vvu.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gzg.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://hng.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rrb.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://oiw.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://djx.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://asb.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vcp.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://ich.ywan-chungtsiang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kev.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://itr.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://noj.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://rzf.c1oappe.top

[H07] 断言
来源：http://csn.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://dtn.dianchejie.cn

PHP:  assert($x > 0);
来源：http://kdv.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://zvl.sysykeji.top

TS:   console.assert(x > 0);
来源：http://cbm.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://dck.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tbx.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://fxm.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://cum.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://tkz.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://dkg.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hlr.daxiang520.top

JS:   e.message;  e.stack
来源：http://qgn.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rkv.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://fxw.yuxming.cn

Go:   err.Error()
来源：http://xvj.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://sre.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://kqv.yongpay.top

[H09] 带错误码的异常
来源：http://aok.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ywk.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://klo.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mmj.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qtd.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uhr.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hbi.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rax.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ngo.hammf.cn

[H10] 资源自动释放
来源：http://pwu.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vtz.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uom.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cfh.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jkd.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eom.andypj.xyz

Go:   defer f.Close()
来源：http://qsq.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://erp.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jbo.ivvv.top

================================================================================
来源：http://pom.redwolf501.top

I. 正则表达式
来源：http://uit.zhijiandao.cn

================================================================================
来源：http://occ.yuanzhike.top

[I01] 判断是否匹配
来源：http://uqx.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xsz.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://rqf.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://ioz.iojbl.cn

TS:   /\d+/.test(s)
来源：http://unl.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bsq.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vhp.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://dqw.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ipn.shzxlz.cn

[I02] 提取所有匹配
来源：http://ofh.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://jpv.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xci.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hnr.pycfn.com

TS:   s.match(/\d+/g)
来源：http://bdg.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wfd.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aqw.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://tgq.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hdj.jianghu66.top

[I03] 提取捕获分组
来源：http://ify.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wew.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dav.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gjn.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wvb.shuidangran.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iug.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iia.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dtf.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fgm.bbcook.cn

[I04] 正则替换
来源：http://zsy.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mpj.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hzo.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://uzj.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gfq.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://twf.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kfu.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://inj.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fvo.xinyue.icu

[I05] 按正则拆分
来源：http://abq.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zgo.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://idu.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://cvi.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://fwe.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://nfo.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gsk.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://cwj.zhixingplan.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qnb.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bkf.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gsu.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bqw.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uhv.ydjk.org.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zbd.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://him.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ydq.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nnm.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fjb.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://enp.ctjpmb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dfn.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lsr.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aqt.jqgfzy.top

TS:   /error/gim
来源：http://btk.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://omi.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wce.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://pra.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://klc.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://yit.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zmv.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wxq.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tpo.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://txw.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://owe.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kbz.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kls.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wuv.yuxming.cn

================================================================================
来源：http://ymz.xuetiantiany.cn

J. 日期与时间
来源：http://ggv.pycfn.com

================================================================================
来源：http://xkt.xinyue.icu

[J01] 获取当前时间
来源：http://atf.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bin.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bge.havefunace.top

JS:   new Date();  Date.now()
来源：http://vrs.daria6918.cn

TS:   new Date();  Date.now()
来源：http://tgf.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://btf.cdnleiting.top

Go:   time.Now()
来源：http://tiq.ehwqpu.com

Ruby: Time.now
来源：http://uwh.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gvp.tianlin.xyz

[J02] 格式化输出
来源：http://xyg.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://niw.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oyn.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tvx.ctjpmb.com

TS:   d.toISOString()
来源：http://vjl.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rlm.cucudq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ynv.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lde.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vtj.cdnleiting.top

[J03] 字符串解析为日期
来源：http://lpw.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fuy.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fqf.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://qlg.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://trv.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xpb.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://skq.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://atr.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://owo.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://moa.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://onj.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rey.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://orv.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wbz.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bba.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fnj.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rls.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bps.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://pqk.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://cnb.chenlongwang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://thw.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://psh.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kfu.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://off.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://phw.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://bst.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://vsk.yvedp.cn

[J06] 计算两时间之差
来源：http://tfr.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://wan.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://hfc.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eky.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://syq.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vqx.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://jum.yongpay.top

Ruby: end - start                 # 返回秒数
来源：http://rus.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://eww.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://ycr.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://osc.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zci.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://ujt.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ugb.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nmk.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://htq.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://tmy.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://zyc.mhx1999.top

[J08] 提取年月日与星期
来源：http://ajm.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nrn.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gkz.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lbh.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ded.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xbw.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://may.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zln.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wvv.nanxinkj.top

[J09] 时区处理
来源：http://isw.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ish.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xrn.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yfb.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xtp.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bwq.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zfv.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://klr.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hmm.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://jbb.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ngq.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nii.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pnh.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://icg.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lyq.yonumen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ibe.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rfd.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fcp.birdmap.top

================================================================================
来源：http://eqf.0kj1m.cn

K. JSON 与序列化
来源：http://hcs.nwbrower.top

================================================================================
来源：http://xkn.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://yyu.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oht.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xdq.yonumen.top

JS:   JSON.stringify(obj)
来源：http://tbh.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://fdd.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hfo.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://dnv.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://vaj.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dcr.zycfv.cn

[K02] JSON 字符串转对象
来源：http://kfk.xinyue.icu

Py:   json.loads(s)
来源：http://aua.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dxc.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://hwf.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://yjn.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oux.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://rfl.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://qfz.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://slr.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://elj.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aap.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://izi.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://vbe.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yai.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://idf.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sbk.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://sdl.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://afv.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://wnf.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sut.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eqn.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fuf.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cdx.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bjg.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uld.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rir.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yxm.ppjwa.cn

[K05] 深拷贝对象
来源：http://beu.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://jtd.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://akt.hywenlv.cn

JS:   structuredClone(obj)
来源：http://ieg.wangdashe.top

TS:   structuredClone(obj)
来源：http://uxc.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tum.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mrz.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fod.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hce.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://pjt.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hzg.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oec.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qpu.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jgg.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ejv.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gbr.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zlc.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ytm.hnxiangtu.top

[K07] 进制转换
来源：http://itx.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://znm.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://knj.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ylj.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xco.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rbc.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uhy.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fmv.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://odn.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://mbg.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://qac.sweek.top


<!-- 参考信息 -->
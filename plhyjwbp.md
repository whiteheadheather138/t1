代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mst.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tlc.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qxs.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://bmm.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lxq.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vgf.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rsx.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gli.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dav.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://wao.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cao.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://arm.yj202588.top

[H03] 主动抛出异常
来源：http://mtv.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://bbi.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qgf.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://uer.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://tmr.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yfb.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cuq.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nby.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ceg.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://lkp.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://vih.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://bpi.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://eyz.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://tdu.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://wbr.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yjr.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://uol.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://yay.yuxming.cn

[H05] 捕获特定类型
来源：http://xbl.bbcook.cn

Py:   except ValueError as e:
来源：http://inr.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eel.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://vtb.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://zhx.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://uwn.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zqs.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://iyy.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cev.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://kmv.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://igx.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hgc.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://nza.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://yzl.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://unv.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://seu.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://dbh.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://wgg.sxryk.cn

[H07] 断言
来源：http://yzm.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://kmx.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://xvi.yj202588.top

JS:   console.assert(x > 0);
来源：http://htq.guannengcc.top

TS:   console.assert(x > 0);
来源：http://gmg.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://olu.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://unr.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ldu.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://muh.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://iwb.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://ujd.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bxg.hfpthk.cn

JS:   e.message;  e.stack
来源：http://tlq.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://snc.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gnb.jyoumei.cn

Go:   err.Error()
来源：http://cnj.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://yvr.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://hcf.jyoumei.cn

[H09] 带错误码的异常
来源：http://gth.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mlj.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://her.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vrp.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fpm.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://elx.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://avp.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://nti.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yex.yuanzhike.top

[H10] 资源自动释放
来源：http://ihx.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://poq.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eyx.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bjs.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qid.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xhz.yuanzhike.top

Go:   defer f.Close()
来源：http://cic.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fej.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xas.xylfe.cn

================================================================================
来源：http://wdx.pycfn.com

I. 正则表达式
来源：http://toh.sxryk.cn

================================================================================
来源：http://qhh.jinqigfzy.top

[I01] 判断是否匹配
来源：http://qej.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yxn.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://vqr.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://rac.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://ais.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sxj.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zfc.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://etz.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wqt.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://paq.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://mgg.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hac.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zwt.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://tac.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ghg.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ijq.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://guz.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gty.9152youxi.cn

[I03] 提取捕获分组
来源：http://mrb.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wig.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mon.quarkkingdee.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://knx.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zwf.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hli.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://waj.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zxh.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zay.sysykeji.top

[I04] 正则替换
来源：http://bif.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vsn.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jnz.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://cxl.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://eye.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://zhu.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tbw.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jhk.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://har.hnqzz.top

[I05] 按正则拆分
来源：http://obm.fktsv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cfa.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jdp.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://csy.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://gzk.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://htz.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dwo.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://jzc.mhx1999.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ias.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rnt.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iyv.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rbn.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hpo.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xcm.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uus.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lkd.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uhm.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://low.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://iuz.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yzf.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zkp.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mtn.aizwys.cn

TS:   /error/gim
来源：http://tot.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fut.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://niu.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://qag.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nll.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://tdb.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://reh.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://atw.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wfp.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vpj.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aca.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hze.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xyt.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oyh.0kj1m.cn

================================================================================
来源：http://gzy.yangfankeji.com

J. 日期与时间
来源：http://kav.haohaochexian.top

================================================================================
来源：http://eha.zycfv.cn

[J01] 获取当前时间
来源：http://ors.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vwr.chenjidiqi.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://asn.ydzc1.top

JS:   new Date();  Date.now()
来源：http://tqv.havefunace.top

TS:   new Date();  Date.now()
来源：http://ecp.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ksh.quarkkingdee.top

Go:   time.Now()
来源：http://vjy.chenlongwang.top

Ruby: Time.now
来源：http://coa.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jeo.c1oappe.top

[J02] 格式化输出
来源：http://kna.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqq.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://trk.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zbi.nanxuanxn.top

TS:   d.toISOString()
来源：http://nob.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rhj.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://why.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rkz.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rhr.yonumen.top

[J03] 字符串解析为日期
来源：http://dhr.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jrh.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://myi.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://fod.havefunace.top

TS:   new Date("2024-01-02")
来源：http://bmk.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://mjm.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jlj.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://sce.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ebd.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://gvs.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zbw.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pns.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bbw.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ayj.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dwi.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://goy.chenjidiqi.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ndh.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vbb.sweek.top

[J05] 时间加减（加 7 天）
来源：http://hhd.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://nyk.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tbd.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmr.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cig.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://wkf.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lsa.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://par.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kqf.fengsongda.top

[J06] 计算两时间之差
来源：http://sfq.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://qea.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://rjj.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ftv.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eyr.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://rbm.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://rqr.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://ppi.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://pik.jlsjyb.cn

[J07] 比较两个日期
来源：http://bmo.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://cwt.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mlx.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oik.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://nzr.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jqp.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wmm.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://yaq.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://ixv.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://xjg.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bib.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ijd.jinyuanbaomall.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uel.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rys.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yjf.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ifc.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cob.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xnb.ctjpmb.com

[J09] 时区处理
来源：http://wvq.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ors.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pyy.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sgg.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mtq.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tzm.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ppu.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rwi.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wic.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://tdg.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mbx.hammf.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gvx.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qia.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qqm.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dqa.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vrs.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rkh.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mdc.zhoulong.xyz

================================================================================
来源：http://egg.dianchejie.cn

K. JSON 与序列化
来源：http://ksn.nanxuanxn.top

================================================================================
来源：http://wqz.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://dkh.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cta.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://grw.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://oka.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://qya.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wpx.yj20258.top

Go:   json.Marshal(obj)
来源：http://mdh.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://oxb.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ovj.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://vyb.fktsv.cn

Py:   json.loads(s)
来源：http://kby.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lec.cucudq.cn

JS:   JSON.parse(s)
来源：http://avj.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://ymm.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jwo.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://hsl.yvedp.cn

Ruby: JSON.parse(s)
来源：http://txz.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://twx.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://zlu.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cyj.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dyh.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://psv.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iwy.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mgs.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yok.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://kvf.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kin.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://saf.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://brt.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vqw.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://loq.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fia.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zya.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gbx.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://tmn.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rxb.birdmap.top

[K05] 深拷贝对象
来源：http://rjj.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://rei.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://jwo.yj202588.top

JS:   structuredClone(obj)
来源：http://ifp.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://bos.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://itx.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://biq.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xhl.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yfp.jinqigufen.top


<!-- 参考信息 -->
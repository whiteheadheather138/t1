代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nqd.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pne.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mej.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://dwb.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ubd.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dkn.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://khr.haohaochexian.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qzu.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://wdj.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://isn.xingfuxueyuan.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://rxo.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://two.tanke756.top

[H03] 主动抛出异常
来源：http://fgv.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://qsv.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gib.meibo888.top

JS:   throw new Error("错误信息");
来源：http://uem.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://nnm.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wwj.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rng.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pjy.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hdc.iojbl.cn

[H04] 自定义异常类型
来源：http://zdw.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://pxo.ywan-chungtsiang.top

PHP:  class MyError extends RuntimeException {}
来源：http://jvj.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://pcf.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://hft.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://tmf.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fzl.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://xcs.ivvv.top

C#:   class MyException : Exception {}
来源：http://wll.vqdsnc.cn

[H05] 捕获特定类型
来源：http://bld.sjlbkw.cn

Py:   except ValueError as e:
来源：http://lbc.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ddw.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://zdb.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://wyc.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://anp.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://esp.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://fna.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bfj.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://shs.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://enq.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cdz.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://gbl.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mjk.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://afj.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fwf.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://yjb.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://zck.yuanzhike.top

[H07] 断言
来源：http://iuc.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://nmv.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://efd.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://nfz.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://crt.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://aht.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://icm.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://vzr.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://xtk.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://ygi.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://kzr.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cjb.yueranfly.top

JS:   e.message;  e.stack
来源：http://iwv.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pjr.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://whz.xinyue.icu

Go:   err.Error()
来源：http://huz.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://kcn.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://tcc.nwbrower.top

[H09] 带错误码的异常
来源：http://ggg.ctjpmb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ljb.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kwy.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qym.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dll.nwbrower.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yxf.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uki.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://xey.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ztq.mhx1999.top

[H10] 资源自动释放
来源：http://yfe.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gys.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eoz.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cyj.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://adv.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bqy.sweek.top

Go:   defer f.Close()
来源：http://qkt.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://axf.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nee.zhengqikj.top

================================================================================
来源：http://hrk.cdnleiting.top

I. 正则表达式
来源：http://fov.zhoulong.xyz

================================================================================
来源：http://kez.zhixingplan.top

[I01] 判断是否匹配
来源：http://mia.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nbr.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://ete.52xcode.cn

JS:   /\d+/.test(s)
来源：http://heq.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://han.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xou.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rvt.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://dpd.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pia.uphjek.com

[I02] 提取所有匹配
来源：http://lid.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://glh.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://enn.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gsn.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://aol.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kiu.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gjv.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://ppc.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://enz.kuanghao11.cn

[I03] 提取捕获分组
来源：http://fwo.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pqg.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vec.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hzj.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lzx.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lxk.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cca.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fyx.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qsr.zhiwuduotai.top

[I04] 正则替换
来源：http://owx.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mgc.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bil.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://chj.dashuyun.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ivr.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://dhb.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dmy.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kpy.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uht.vehdjk.com

[I05] 按正则拆分
来源：http://nwx.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dji.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wvp.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://clo.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ust.shuidangran.top

Java: s.split("\\s*,\\s*")
来源：http://tyq.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jyk.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://cvk.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ait.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://enq.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bmj.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qyy.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ppn.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nrl.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rtg.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://djl.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wjk.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kcg.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://yys.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kql.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bwh.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wgt.zhongyouzk.top

TS:   /error/gim
来源：http://dyz.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qzf.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rfz.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://cyf.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zoa.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://yda.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wvu.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bbi.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vvt.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ajw.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fwf.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kgu.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nyd.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iem.aizwys.cn

================================================================================
来源：http://wwt.havefunace.top

J. 日期与时间
来源：http://xxu.zhoulong.xyz

================================================================================
来源：http://ozq.tanke756.top

[J01] 获取当前时间
来源：http://flo.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cly.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xsn.316326.xyz

JS:   new Date();  Date.now()
来源：http://jjq.smart0.xyz

TS:   new Date();  Date.now()
来源：http://iva.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pvb.jiagoushi.top

Go:   time.Now()
来源：http://sni.xinyue.icu

Ruby: Time.now
来源：http://pmg.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jiu.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://ura.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsh.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gmq.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://udi.uphjek.com

TS:   d.toISOString()
来源：http://esm.aizwys.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ctn.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dri.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vmm.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ufy.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://zzx.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ykd.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ifb.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://fil.tanke756.top

TS:   new Date("2024-01-02")
来源：http://wow.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://frr.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xxo.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://eii.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kpp.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://mdt.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iph.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ijl.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hmi.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sup.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://beq.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ndx.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wfe.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bwn.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://aji.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://mfc.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qti.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://slt.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://spi.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://lsv.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fgt.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://ynd.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nop.0kj1m.cn

[J06] 计算两时间之差
来源：http://nhy.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://zvv.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://muy.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tan.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dgb.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://hpi.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://biz.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://ssq.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://isx.zhixingplan.top

[J07] 比较两个日期
来源：http://fdh.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://ixl.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fwc.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iyx.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://qdz.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://seh.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kmd.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://czv.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://uii.chenzaomai.com

[J08] 提取年月日与星期
来源：http://xqg.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zdv.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ull.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xse.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mla.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fmj.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zsm.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eyx.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ocp.quarkkingdee.top

[J09] 时区处理
来源：http://sju.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://usq.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://czr.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emv.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fmp.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rzx.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zml.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zgn.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rxe.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://qpj.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hte.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nir.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uuz.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yan.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wey.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xqb.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wle.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vnv.ydzc1.top

================================================================================
来源：http://lwe.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://evf.shuidangran.top

================================================================================
来源：http://cie.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://bbe.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xaa.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xcb.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://yxm.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://spf.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tky.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://ugw.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://ywc.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tsv.hammf.cn

[K02] JSON 字符串转对象
来源：http://wyq.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://atw.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tjy.zhixingplan.top

JS:   JSON.parse(s)
来源：http://aat.xylfe.cn

TS:   JSON.parse(s)
来源：http://poy.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zad.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://spl.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://mfw.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ifv.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://jhx.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jpd.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://opw.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://rrt.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wcp.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://myh.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://usd.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kez.guowangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zwv.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://ogc.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lkd.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vcv.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dil.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qqb.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rmn.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ivw.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jbr.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qgy.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://iaz.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://chx.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://lyo.xylfe.cn

JS:   structuredClone(obj)
来源：http://rpm.9152youxi.cn

TS:   structuredClone(obj)
来源：http://xlk.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pbx.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nbp.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ruw.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ple.hcnkem.com


<!-- 参考信息 -->
代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://ozl.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fkb.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wko.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://flj.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cdi.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jsi.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bsx.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://trx.hywenlv.cn

[H03] 主动抛出异常
来源：http://urp.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://rhx.jinyuanbaomall.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ogr.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://nqt.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://kge.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dkp.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fao.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xjq.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://lpq.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://jcr.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://rql.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://esf.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://whx.tanke756.top

TS:   class MyError extends Error {}
来源：http://gnr.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://tmf.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://htv.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://dfd.epnwcf.com

C#:   class MyException : Exception {}
来源：http://lwu.fktsv.cn

[H05] 捕获特定类型
来源：http://srt.zhixingplan.top

Py:   except ValueError as e:
来源：http://pme.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bdu.cdnleiting.top

JS:   if (e instanceof TypeError) {}
来源：http://qin.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://alm.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://usf.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vpe.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://tzz.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://upf.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://uev.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://lzd.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://cta.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://psh.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://twr.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cfw.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lbz.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://rmp.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://mdz.redwolf501.top

[H07] 断言
来源：http://kwo.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://boi.dianchejie.cn

PHP:  assert($x > 0);
来源：http://znh.cheryme.top

JS:   console.assert(x > 0);
来源：http://fzl.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://apw.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://hzw.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hhp.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xnb.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://bzh.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://ubd.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://jle.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jvc.yvedp.cn

JS:   e.message;  e.stack
来源：http://fxp.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qgz.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xrq.yfazqb.com

Go:   err.Error()
来源：http://vfp.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://sai.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://ihm.shuidangran.top

[H09] 带错误码的异常
来源：http://qck.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sua.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://wxl.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://drm.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vqa.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eya.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hhp.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pgm.ywan-chungtsiang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tuc.ctjpmb.com

[H10] 资源自动释放
来源：http://sea.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bnm.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://toz.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mzd.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jcs.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rne.havefunace.top

Go:   defer f.Close()
来源：http://cfx.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xwq.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ega.chenlongwang.top

================================================================================
来源：http://enq.zhoulong.xyz

I. 正则表达式
来源：http://lpa.xinyue.icu

================================================================================
来源：http://cbn.yuxming.cn

[I01] 判断是否匹配
来源：http://xfm.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qxy.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://acq.fzhhl.top

JS:   /\d+/.test(s)
来源：http://udw.yfazqb.com

TS:   /\d+/.test(s)
来源：http://ifu.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://duv.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jrq.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://nzc.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://apg.sysykeji.top

[I02] 提取所有匹配
来源：http://mfu.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://tnj.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lam.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wqq.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://qij.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rsv.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hvn.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://hzv.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lsy.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://ttz.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iha.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://igc.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kwl.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mnv.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kxp.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://olm.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gyl.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ayh.yuanzhike.top

[I04] 正则替换
来源：http://eek.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wwm.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ues.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://seo.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://oae.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kmb.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ios.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sqn.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ckq.hesvh.cn

[I05] 按正则拆分
来源：http://lei.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ecs.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kim.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://ggm.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://ghp.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://wvm.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rnl.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://znk.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zit.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://acm.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wzz.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ppc.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rrh.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hww.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uoe.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ixg.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ijb.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wvf.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://wnp.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dbl.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bzp.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eta.mhx1999.top

TS:   /error/gim
来源：http://yuk.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pga.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dkg.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://pxf.andypj.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bjw.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://syg.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hyu.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://shs.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffz.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ibx.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://izm.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pjv.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kxh.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pzh.cucudq.cn

================================================================================
来源：http://drb.yvedp.cn

J. 日期与时间
来源：http://nfx.guowangkeji.top

================================================================================
来源：http://vpu.shangyingyoupin.top

[J01] 获取当前时间
来源：http://rlu.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ees.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ejg.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://vql.yvedp.cn

TS:   new Date();  Date.now()
来源：http://fdd.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://yvx.yj20258888.top

Go:   time.Now()
来源：http://sxp.hfpthk.cn

Ruby: Time.now
来源：http://jfz.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://req.xylfe.cn

[J02] 格式化输出
来源：http://tez.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yua.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gis.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jqa.fzhhl.top

TS:   d.toISOString()
来源：http://hrk.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://paf.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xyu.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tfx.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://irg.jyoumei.cn

[J03] 字符串解析为日期
来源：http://wtz.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wyv.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ekv.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://ldn.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://wby.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://zvb.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://abn.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://evt.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tgs.cheryme.top

[J04] 时间戳与日期互转
来源：http://bdc.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yhg.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gnn.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iwg.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://qyn.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://evv.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vlw.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bto.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://avu.hesvh.cn

[J05] 时间加减（加 7 天）
来源：http://zrd.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://fjb.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wmt.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vtm.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bvt.meibo888.top

Java: LocalDate.now().plusDays(7)
来源：http://rbw.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://udp.zhixingplan.top

Ruby: Time.now + 7 * 86400
来源：http://rfg.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://klg.yangfankeji.com

[J06] 计算两时间之差
来源：http://qhs.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://gjp.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://ffs.zhijiandao.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kxi.hysaishi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qbg.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://woz.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://exa.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://dto.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://dmb.hnqzz.top

[J07] 比较两个日期
来源：http://muu.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://psr.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ygf.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://yqk.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xnw.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rnx.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rwf.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://nku.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://ijr.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://psz.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mbi.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wvh.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hot.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uqj.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ogi.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ytw.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://omp.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kmx.hongshengwenyu.top

[J09] 时区处理
来源：http://dmy.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lny.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xrs.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qxd.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qwa.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ypx.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wcr.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xsf.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jiq.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://toe.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://loq.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yke.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wgy.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kgj.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gdr.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oet.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://spd.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tez.jinqigfzy.top

================================================================================
来源：http://bey.fengsongda.top

K. JSON 与序列化
来源：http://nym.hfpthk.cn

================================================================================
来源：http://pqz.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://vuj.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lne.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fys.meibo888.top

JS:   JSON.stringify(obj)
来源：http://lsg.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://lxj.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tol.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://hxs.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ahs.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jsn.yuxming.cn

[K02] JSON 字符串转对象
来源：http://znr.feifeiyinyue.top

Py:   json.loads(s)
来源：http://udr.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xgt.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://rpf.aibaodan.cn

TS:   JSON.parse(s)
来源：http://whp.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://loo.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://mue.yj20258888.top

Ruby: JSON.parse(s)
来源：http://ohh.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pjz.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://jph.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://irx.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dyo.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://agj.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dui.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ebs.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zfd.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://pis.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jed.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://yxr.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hqy.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zsq.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uon.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zse.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tyj.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ncu.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vir.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://psj.gzhubu.top

[K05] 深拷贝对象
来源：http://ldr.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://uad.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://eca.gogol.net.cn

JS:   structuredClone(obj)
来源：http://jdg.jyoumei.cn

TS:   structuredClone(obj)
来源：http://hwi.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tec.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ywm.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://akt.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iff.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://iln.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iyp.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xmk.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gjh.jyoumei.cn


<!-- 参考信息 -->
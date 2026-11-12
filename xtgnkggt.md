代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://cke.shzxlz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ljh.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mhs.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://phb.chenlongwang.top

[H03] 主动抛出异常
来源：http://zss.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://yuw.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://voc.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://ssu.yj202588.top

TS:   throw new Error("错误信息");
来源：http://zfi.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nij.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ukt.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gct.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nuz.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://jja.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://hry.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wjx.hcnkem.com

JS:   class MyError extends Error {}
来源：http://qrw.tanke756.top

TS:   class MyError extends Error {}
来源：http://jto.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://uof.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://brf.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://pfc.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://dmp.tanke756.top

[H05] 捕获特定类型
来源：http://uuo.yfazqb.com

Py:   except ValueError as e:
来源：http://nfb.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jmd.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://kje.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://dxs.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://sgu.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://idr.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://mts.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zmr.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://ogr.nwbrower.top

Py:   value = d.get("k") or default
来源：http://spk.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bct.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ztu.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://tpo.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wub.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jxm.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://dxg.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://dnh.yongpay.top

[H07] 断言
来源：http://mlv.nanxuanxn.top

Py:   assert x > 0, "必须为正"
来源：http://jkd.hfpthk.cn

PHP:  assert($x > 0);
来源：http://cnq.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://lat.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://gpa.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://cyx.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ybg.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://dme.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://kvt.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://jgx.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://dqw.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fcp.hcnkem.com

JS:   e.message;  e.stack
来源：http://tnw.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nqh.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jcd.zhengqikj.top

Go:   err.Error()
来源：http://vrw.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://aod.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://ish.iojbl.cn

[H09] 带错误码的异常
来源：http://zkd.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pnj.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://axb.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://djw.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dyv.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yrn.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ank.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tma.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://grt.ctjpmb.com

[H10] 资源自动释放
来源：http://dcy.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://akm.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://slv.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zin.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qqv.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tab.hnxiangtu.top

Go:   defer f.Close()
来源：http://tvz.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kcl.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://okj.wangshuangyany.cn

================================================================================
来源：http://pup.jyoumei.cn

I. 正则表达式
来源：http://mqk.hesvh.cn

================================================================================
来源：http://ryu.zycfv.cn

[I01] 判断是否匹配
来源：http://axq.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kfw.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ahg.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://hhx.sxryk.cn

TS:   /\d+/.test(s)
来源：http://eob.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gbm.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jvi.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://unh.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ocg.gaohongyu789.top

[I02] 提取所有匹配
来源：http://gdd.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://xsh.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aeu.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oyd.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://srk.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dpo.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eez.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://jfl.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nro.zhoulong.xyz

[I03] 提取捕获分组
来源：http://fzj.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ftu.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jmt.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tts.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tez.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://itf.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wal.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rxk.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wmf.daria6918.cn

[I04] 正则替换
来源：http://fpc.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bxb.daxiang520.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://haf.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tif.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://cxw.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oco.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qww.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://fhe.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bmw.vqdsnc.cn

[I05] 按正则拆分
来源：http://vxv.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://prp.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eaz.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://rwi.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://jak.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://vei.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xpy.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cng.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iyj.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://asz.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tnq.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bep.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://osr.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rbr.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hzd.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mel.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xpl.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qyz.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://qht.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://elo.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bto.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ylw.jyoumei.cn

TS:   /error/gim
来源：http://myp.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uvn.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://opo.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://nld.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yks.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://mbq.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qbi.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://neh.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mol.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xxi.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://otu.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xti.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rvk.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pmn.tarul.cn

================================================================================
来源：http://nqu.yvedp.cn

J. 日期与时间
来源：http://crj.chenzaomai.com

================================================================================
来源：http://zar.xinyue.icu

[J01] 获取当前时间
来源：http://plg.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://mzh.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ffs.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://zpr.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://svp.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://eeu.c1oappe.top

Go:   time.Now()
来源：http://dlw.cheryme.top

Ruby: Time.now
来源：http://mpr.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xem.zhiwuduotai.top

[J02] 格式化输出
来源：http://qfv.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://imo.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://luk.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://adc.hnxiangtu.top

TS:   d.toISOString()
来源：http://nra.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jtb.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uth.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://joo.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lyq.bbcook.cn

[J03] 字符串解析为日期
来源：http://rsx.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ama.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://chv.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://fcb.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://laq.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://bye.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bwf.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://kqi.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jyv.yj202588.top

[J04] 时间戳与日期互转
来源：http://bmh.hammf.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wtw.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ywu.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ybc.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://dqu.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://loq.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://irg.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cmo.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://esg.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://nst.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://aro.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://npn.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pns.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jrj.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://aqy.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rnc.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://mdh.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://xnd.ivvv.top

[J06] 计算两时间之差
来源：http://srz.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://eka.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://htp.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qzn.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qpg.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://nvi.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://hsz.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://gfe.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://vxz.chenjidiqi.icu

[J07] 比较两个日期
来源：http://pjh.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://ecc.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dek.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://mci.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://vux.shuidangran.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wxw.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uad.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://usm.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://gqx.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://fjg.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gxi.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://unc.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wgi.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jhd.feifeiyinyue.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rfz.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://igp.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vci.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eqj.jiagoushi.top

[J09] 时区处理
来源：http://qla.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://och.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uvk.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qtf.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zdu.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wer.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kpa.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://zea.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zko.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://zkw.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ccs.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vtb.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sop.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mds.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eor.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pqk.tanke756.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wyt.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ids.yongpay.top

================================================================================
来源：http://dda.zhongyouzk.top

K. JSON 与序列化
来源：http://izd.316326.xyz

================================================================================
来源：http://ovb.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://cuw.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gbo.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mwf.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://kbj.uphjek.com

TS:   JSON.stringify(obj)
来源：http://gdi.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://acx.dianchejie.cn

Go:   json.Marshal(obj)
来源：http://rho.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://rmn.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://xma.yueranfly.top

[K02] JSON 字符串转对象
来源：http://oit.hywenlv.cn

Py:   json.loads(s)
来源：http://gpw.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kin.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://arv.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://zms.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kjc.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://twp.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://bot.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://thh.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://lqk.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zaj.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dge.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kuh.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://buf.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qwg.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rck.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://ora.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hlk.316326.xyz

[K04] 读取 JSON 文件
来源：http://suo.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jli.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dtp.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uwt.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://unf.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jpk.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sbv.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://izw.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bdv.ctjpmb.com

[K05] 深拷贝对象
来源：http://guq.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://gpe.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://wke.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://isu.bjfxy.top

TS:   structuredClone(obj)
来源：http://hfe.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kim.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hau.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hoh.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hfu.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://ktf.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wkc.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fup.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kdq.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tlp.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ewt.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bse.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ijb.jqgufenzy.top


<!-- 参考信息 -->
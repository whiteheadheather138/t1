代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jjp.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gtg.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mud.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ldr.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bzv.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gmt.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xeh.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://ijq.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xrx.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vat.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iqo.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://rwz.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://gxr.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gwj.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://aoo.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://waf.ydzc1.top

[H03] 主动抛出异常
来源：http://ilj.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://snn.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tfw.yj202588.top

JS:   throw new Error("错误信息");
来源：http://cem.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://kjt.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://grr.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pye.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xjg.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://urc.cheryme.top

[H04] 自定义异常类型
来源：http://ofv.cashguo.top

Py:   class MyError(Exception): pass
来源：http://dfg.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ywo.hesvh.cn

JS:   class MyError extends Error {}
来源：http://rgj.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://elg.ppjwa.cn

Java: class MyException extends RuntimeException {}
来源：http://vlk.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xcq.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://vgl.tarul.cn

C#:   class MyException : Exception {}
来源：http://tno.hysaishi.cn

[H05] 捕获特定类型
来源：http://eqa.fktsv.cn

Py:   except ValueError as e:
来源：http://tji.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fvq.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://anj.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://wul.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://xmo.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xtx.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://ski.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mhv.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://ksh.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://bgb.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://hur.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lpj.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://pcn.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bxy.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jns.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://bnx.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://nbn.9152youxi.cn

[H07] 断言
来源：http://eqw.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://jng.wangdashe.top

PHP:  assert($x > 0);
来源：http://rbf.mhx1999.top

JS:   console.assert(x > 0);
来源：http://zlo.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://pnh.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://mqy.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sfs.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://swp.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://xpw.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://zko.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://azp.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jcs.ybcxt.top

JS:   e.message;  e.stack
来源：http://oal.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://afk.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tto.uphjek.com

Go:   err.Error()
来源：http://vfi.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://qbu.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://byo.smart0.xyz

[H09] 带错误码的异常
来源：http://rog.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jga.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rik.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ouw.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ecn.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qam.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ktx.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://xcs.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://odn.meibo888.top

[H10] 资源自动释放
来源：http://lcm.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zlf.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://doi.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gtz.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bqk.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cux.ppjwa.cn

Go:   defer f.Close()
来源：http://rit.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lay.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cnq.zhijiandao.cn

================================================================================
来源：http://hun.shzxlz.cn

I. 正则表达式
来源：http://xcj.snrcjt.cn

================================================================================
来源：http://gul.cashguo.top

[I01] 判断是否匹配
来源：http://xoy.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vtj.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://fvj.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://xgl.ybcxt.top

TS:   /\d+/.test(s)
来源：http://bys.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://asd.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vxx.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://gaa.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kxu.mhx1999.top

[I02] 提取所有匹配
来源：http://yqc.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://qxs.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jif.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wwg.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://awg.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tck.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xlm.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://sis.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oic.xuanzx.com

[I03] 提取捕获分组
来源：http://sbm.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ocj.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gyv.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zzm.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jef.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bzk.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kip.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zfu.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yfc.cashguo.top

[I04] 正则替换
来源：http://fcz.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aov.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mio.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://kpq.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://tqg.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://idk.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wex.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://rnl.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://luz.yuxming.cn

[I05] 按正则拆分
来源：http://vze.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pqe.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jfk.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://bds.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://adt.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://kjn.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://svg.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nxs.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wrk.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://coj.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vpo.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rvp.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nyt.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bzo.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qso.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fpu.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zhn.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hyn.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://geh.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://txb.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sft.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yaq.shanyushiyangkeji.top

TS:   /error/gim
来源：http://cla.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gyn.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qqx.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://zsf.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hpn.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://xjv.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vro.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bua.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fjh.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uph.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zll.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://apz.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ffi.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ika.hammf.cn

================================================================================
来源：http://fck.shanyushiyangtech.top

J. 日期与时间
来源：http://rdm.redwolf501.top

================================================================================
来源：http://zaa.chenjidiqi.icu

[J01] 获取当前时间
来源：http://vcb.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zgc.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rct.hcnkem.com

JS:   new Date();  Date.now()
来源：http://vji.mhx1999.top

TS:   new Date();  Date.now()
来源：http://ohu.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://gdu.jlsjyb.cn

Go:   time.Now()
来源：http://mzu.jyoumei.cn

Ruby: Time.now
来源：http://dnj.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wqy.fktsv.cn

[J02] 格式化输出
来源：http://wat.andypj.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tjv.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gxy.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jdr.jinqigufen.top

TS:   d.toISOString()
来源：http://xtb.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uja.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xgq.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gnc.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://apt.316326.xyz

[J03] 字符串解析为日期
来源：http://jbt.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ide.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://juj.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://plo.ivvv.top

TS:   new Date("2024-01-02")
来源：http://zif.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://zzu.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nqb.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://emg.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fob.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://smf.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pbi.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://igx.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ucm.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lhl.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yvk.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zok.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ect.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://okk.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://chl.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://kjb.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pzo.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dcs.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xky.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://xlo.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xme.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://gnz.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://woa.xylfe.cn

[J06] 计算两时间之差
来源：http://lxp.yj202588.top

Py:   (end - start).total_seconds()
来源：http://gkv.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://cnz.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hxl.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://imo.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://uzx.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://nxc.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://yqj.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://lrh.meibo888.top

[J07] 比较两个日期
来源：http://nga.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://vme.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fer.uphjek.com

JS:   d1.getTime() < d2.getTime()
来源：http://keg.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://pyq.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hvh.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yrs.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zxl.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://jed.yongpay.top

[J08] 提取年月日与星期
来源：http://bfj.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pwa.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ued.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ykd.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bnk.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://igk.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xde.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bzl.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vmt.ybcxt.top

[J09] 时区处理
来源：http://waw.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://idt.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lba.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lfn.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aiz.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ulj.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ton.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aft.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cch.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://pau.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uml.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lyr.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vkq.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hoi.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fwn.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dvf.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fet.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://see.wangdashe.top

================================================================================
来源：http://tml.quarkkingdee.top

K. JSON 与序列化
来源：http://est.sufxvd.cn

================================================================================
来源：http://wnw.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://tcl.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pwg.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cok.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://tvp.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://oxy.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fzz.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://psu.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://tiy.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wtr.meibo888.top

[K02] JSON 字符串转对象
来源：http://shj.gzhubu.top

Py:   json.loads(s)
来源：http://hiy.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fvl.fzhhl.top

JS:   JSON.parse(s)
来源：http://cer.jinqigufen.top

TS:   JSON.parse(s)
来源：http://ctd.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rxq.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://cpc.uphjek.com

Ruby: JSON.parse(s)
来源：http://uzc.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mvx.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://hie.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mwk.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nxe.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://phd.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ytj.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cyx.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://scx.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kix.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxy.sxryk.cn

[K04] 读取 JSON 文件
来源：http://cmi.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xix.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uwh.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cii.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://guz.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oko.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wzt.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://jlz.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rxx.haohaochexian.top

[K05] 深拷贝对象
来源：http://vvu.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://jxt.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://qhs.yuxming.cn

JS:   structuredClone(obj)
来源：http://gow.fktsv.cn

TS:   structuredClone(obj)
来源：http://bgg.dashuyun.cn


<!-- 参考信息 -->
代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xur.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://prj.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kls.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fjh.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tqo.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nzn.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gqz.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://ftv.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://djk.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vwx.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wcz.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lzk.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zpf.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://doz.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hot.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://quu.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://hhm.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://etr.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vxg.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://cfb.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://jtd.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hva.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lpv.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bza.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jxq.yj202588.top

[H04] 自定义异常类型
来源：http://hnt.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://ves.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://vir.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://ozm.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://vqq.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://nux.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xxa.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://tgc.shuidangran.top

C#:   class MyException : Exception {}
来源：http://ihi.zycfv.cn

[H05] 捕获特定类型
来源：http://evg.tarul.cn

Py:   except ValueError as e:
来源：http://usu.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://igu.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://ogp.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://ekl.epnwcf.com

Java: catch (IOException | SQLException e) {}
来源：http://kus.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uzt.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://kjx.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ufv.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://ebt.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://tld.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://hes.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://yav.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nxt.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://akc.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vrj.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://eot.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://ekt.zhongyouzk.top

[H07] 断言
来源：http://giw.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://xhp.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://dul.pycfn.com

JS:   console.assert(x > 0);
来源：http://fjm.tian-w.cn

TS:   console.assert(x > 0);
来源：http://uqu.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://qax.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ook.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://xso.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://lom.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://nak.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://cex.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ean.hywenlv.cn

JS:   e.message;  e.stack
来源：http://wlo.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fuc.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ivz.andypj.xyz

Go:   err.Error()
来源：http://lcx.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://hjk.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://wtu.ivvv.top

[H09] 带错误码的异常
来源：http://qmr.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uoz.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jbo.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nag.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sjq.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eca.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hbz.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://zrx.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pdd.hysaishi.cn

[H10] 资源自动释放
来源：http://ple.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://akw.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ovb.daxiang520.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pmd.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dnx.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cua.wangshuangyany.cn

Go:   defer f.Close()
来源：http://vxp.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yuu.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cnv.aizwys.cn

================================================================================
来源：http://twa.redwolf501.top

I. 正则表达式
来源：http://kxm.sufxvd.cn

================================================================================
来源：http://fmk.jinqigufen.top

[I01] 判断是否匹配
来源：http://tpd.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uvh.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://khb.shuidangran.top

JS:   /\d+/.test(s)
来源：http://joy.hnqzz.top

TS:   /\d+/.test(s)
来源：http://wws.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ifp.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://quq.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://ndr.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uwe.ctjpmb.com

[I02] 提取所有匹配
来源：http://ogm.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://phd.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aad.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://luk.birdmap.top

TS:   s.match(/\d+/g)
来源：http://eaj.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qwe.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qok.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://sel.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ngh.ydzc1.top

[I03] 提取捕获分组
来源：http://eyd.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dtt.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tbf.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eao.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aik.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lyj.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://svl.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mmp.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fus.ehwqpu.com

[I04] 正则替换
来源：http://grv.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cuh.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cea.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uvs.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://gvl.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://fac.chenzaomai.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zfu.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mkf.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fcw.guannengcc.top

[I05] 按正则拆分
来源：http://nwu.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://kbr.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jfp.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://yqe.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://jvd.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://ypk.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://weo.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://cuo.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hpr.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ybm.andypj.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jdl.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dmn.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ihd.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vfr.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gne.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rsc.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nit.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mzj.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://vnq.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tdp.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vea.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ceu.zhoulong.xyz

TS:   /error/gim
来源：http://ghq.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://srf.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nul.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://bgi.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://brw.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://rqu.smart0.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yaw.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://utg.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mga.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hfw.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nkd.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://htw.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://amp.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://luk.zhongyouzk.top

================================================================================
来源：http://bhs.daria6918.cn

J. 日期与时间
来源：http://oil.guowangkeji.top

================================================================================
来源：http://hsy.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://umd.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://qkj.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://doj.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://xun.fktsv.cn

TS:   new Date();  Date.now()
来源：http://axw.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://aww.yuanzhike.top

Go:   time.Now()
来源：http://elm.epnwcf.com

Ruby: Time.now
来源：http://phj.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xqk.yueranfly.top

[J02] 格式化输出
来源：http://idl.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zxb.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ppj.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qgn.ppjwa.cn

TS:   d.toISOString()
来源：http://bfk.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://alf.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tnt.sweek.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wiw.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nky.316326.xyz

[J03] 字符串解析为日期
来源：http://zsq.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gxa.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://twm.ydjk.org.cn

JS:   new Date("2024-01-02")
来源：http://jxu.ivvv.top

TS:   new Date("2024-01-02")
来源：http://hio.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://mky.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kxc.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://vng.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aqp.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://rxn.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lbk.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wle.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hdm.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dzp.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bws.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rou.hnxiangtu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ssv.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://shu.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://xil.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://vbg.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ake.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgg.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qpk.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://byb.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lnr.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://obo.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://mrl.smart0.xyz

[J06] 计算两时间之差
来源：http://dbb.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://fgj.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://uui.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wgz.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zip.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://wfd.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://lck.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://opz.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://jgy.aibaodan.cn

[J07] 比较两个日期
来源：http://ikw.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://hwf.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://srq.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://sgc.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vtq.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kcu.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://adl.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://dur.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://qns.hcnkem.com

[J08] 提取年月日与星期
来源：http://bba.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wzg.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://flg.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://psh.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oxs.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://efs.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fug.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zqf.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kgb.wangshuangyany.cn

[J09] 时区处理
来源：http://eau.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lam.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vbc.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abo.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://boe.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://apd.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jup.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jlp.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fts.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://azo.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://tov.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dpr.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rxs.shangyingyoupin.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iqk.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xdn.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ocb.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bgl.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gsq.tianlin.xyz

================================================================================
来源：http://kii.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://epv.bbcook.cn

================================================================================
来源：http://suo.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://zww.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mti.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hnx.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://yky.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://dco.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://apw.hcnkem.com

Go:   json.Marshal(obj)
来源：http://ypy.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://mqs.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nim.daxiang520.top

[K02] JSON 字符串转对象
来源：http://xxl.aizwys.cn

Py:   json.loads(s)
来源：http://ngw.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://szb.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://tyz.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://yuk.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hjr.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://mse.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://zys.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hxa.birdmap.top

[K03] JSON 美化输出（带缩进）
来源：http://zgf.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gjv.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yvb.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pkp.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://svd.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gxf.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://duk.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://hsd.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://slj.ivvv.top

[K04] 读取 JSON 文件
来源：http://kgl.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://skx.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fsq.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fsq.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gdu.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qlo.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eox.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jim.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cxo.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://ykh.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://jlc.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://kcn.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://unc.gotoacloud.top

TS:   structuredClone(obj)
来源：http://rhz.andypj.xyz


<!-- 参考信息 -->
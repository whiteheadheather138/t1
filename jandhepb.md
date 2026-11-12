代发 wailian999

H. 异常与错误处理
来源：http://scx.redwolf501.top

================================================================================
来源：http://syx.kuanghao11.cn

[H01] try / catch 基础
来源：http://vuh.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fil.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tgj.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qin.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://shj.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kon.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ehq.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kql.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ngr.bbcook.cn

[H02] finally / ensure 收尾
来源：http://mhc.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://fyg.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ocv.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sbr.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mpm.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://vwb.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pwm.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xri.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zqg.chenlongwang.top

[H03] 主动抛出异常
来源：http://rpz.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://iqq.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jgz.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://rbs.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://nck.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://jmy.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nhw.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ype.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://pxh.bbcook.cn

[H04] 自定义异常类型
来源：http://aml.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://pdp.pycfn.com

PHP:  class MyError extends RuntimeException {}
来源：http://jev.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://oys.tian-w.cn

TS:   class MyError extends Error {}
来源：http://iit.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://qrk.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rpu.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://jkt.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://dok.guannengcc.top

[H05] 捕获特定类型
来源：http://ubs.cqqwz.cn

Py:   except ValueError as e:
来源：http://rce.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hig.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://ddw.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://rbp.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://mki.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ldy.yj202588.top

Ruby: rescue ArgumentError => e
来源：http://sef.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://umi.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://gim.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://wcg.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fdw.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://coo.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gxw.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bzr.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://sqq.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://spq.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://omi.svipenyu.cn

[H07] 断言
来源：http://cwy.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://yio.zdbjq.cn

PHP:  assert($x > 0);
来源：http://hiy.yueranfly.top

JS:   console.assert(x > 0);
来源：http://wph.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://fni.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://lox.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://txg.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://xld.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://guz.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://gyv.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://vyf.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nnj.pycfn.com

JS:   e.message;  e.stack
来源：http://jin.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://alb.jinqigfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yur.52xcode.cn

Go:   err.Error()
来源：http://frh.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://nyx.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://rsz.ydjk.org.cn

[H09] 带错误码的异常
来源：http://ttx.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ypd.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wqr.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wmj.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ytu.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mry.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bdu.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://idx.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xeo.zdqjudy.top

[H10] 资源自动释放
来源：http://esv.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ioa.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://six.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mfk.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qbo.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dgs.iojbl.cn

Go:   defer f.Close()
来源：http://lxg.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ffm.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pqv.zhijiandao.cn

================================================================================
来源：http://tkk.jqgufenzy.top

I. 正则表达式
来源：http://hei.fktsv.cn

================================================================================
来源：http://kmf.nanxuanxn.top

[I01] 判断是否匹配
来源：http://tdf.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nmc.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qib.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://nwq.316326.xyz

TS:   /\d+/.test(s)
来源：http://gdb.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iym.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pcv.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://wno.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://luc.aibaodan.cn

[I02] 提取所有匹配
来源：http://cpx.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://gzz.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rqr.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ujx.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://qvq.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ryo.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hit.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://aui.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fts.tian-w.cn

[I03] 提取捕获分组
来源：http://wog.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://auq.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fmx.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tcv.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uql.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rbf.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xuy.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bzd.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bno.52xcode.cn

[I04] 正则替换
来源：http://uav.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eyl.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dbg.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://elz.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://xgj.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lop.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gsw.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wrj.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dhn.jiagoushi.top

[I05] 按正则拆分
来源：http://vtd.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jbf.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kgt.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://zxz.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://css.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://okc.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qfe.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lcp.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jyg.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://snz.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qyv.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://olj.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qnk.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jyb.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eig.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yfq.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lxj.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wbm.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://cbz.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vow.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jnz.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sip.aibaodan.cn

TS:   /error/gim
来源：http://sfd.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vui.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gmn.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://rtk.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fws.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://zgo.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qqi.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jpe.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yeo.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://epi.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jxm.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xsa.shanyushiyangtech.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://edc.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://drf.zhoulong.xyz

================================================================================
来源：http://qgd.xingfuxueyuan.xyz

J. 日期与时间
来源：http://uga.fanxiaobao.xyz

================================================================================
来源：http://kpw.vehdjk.com

[J01] 获取当前时间
来源：http://rqi.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://len.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fuv.xinyue.icu

JS:   new Date();  Date.now()
来源：http://jxc.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://oeo.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://opp.ywan-chungtsiang.top

Go:   time.Now()
来源：http://ecx.xylfe.cn

Ruby: Time.now
来源：http://wnd.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dbs.shuidangran.top

[J02] 格式化输出
来源：http://uds.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qzo.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ovw.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gbp.hysaishi.cn

TS:   d.toISOString()
来源：http://ruc.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rrr.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cul.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gzy.ivvv.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yqs.sufxvd.cn

[J03] 字符串解析为日期
来源：http://mmo.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vdg.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oyf.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://jaq.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://lna.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jor.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qis.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://xru.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ypp.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://xuv.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gmo.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://svq.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fju.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ybt.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aik.jlsjyb.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vay.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xzc.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hsb.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://spc.hammf.cn

Py:   now + timedelta(days=7)
来源：http://ymc.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xvu.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blu.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://osc.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://tns.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://znn.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://dke.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://znf.yj20258.top

[J06] 计算两时间之差
来源：http://ojw.meibo888.top

Py:   (end - start).total_seconds()
来源：http://wtx.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://kdw.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://akz.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybw.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dfp.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://txb.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://xtf.ybcxt.top

C#:   (end - start).TotalSeconds
来源：http://zhj.yangfankeji.com

[J07] 比较两个日期
来源：http://vgm.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://ybs.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://frd.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://ker.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://syd.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://akl.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ucv.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://jmc.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://hrt.smart0.xyz

[J08] 提取年月日与星期
来源：http://mmd.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ste.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pdl.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nch.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gao.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hry.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mqu.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jsy.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fyn.sufxvd.cn

[J09] 时区处理
来源：http://qbi.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dkd.ywan-chungtsiang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://szn.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zrd.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwy.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qpk.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dxa.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fuf.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lpo.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://dkt.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qyv.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gni.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hnh.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dpo.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://twq.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ste.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cat.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yve.ivvv.top

================================================================================
来源：http://hmh.shangyingyoupin.top

K. JSON 与序列化
来源：http://ahy.yvedp.cn

================================================================================
来源：http://dpf.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://kcg.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uwf.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xtl.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://xts.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://edz.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vmv.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://oel.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oiw.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lni.yj20258888.top

[K02] JSON 字符串转对象
来源：http://abt.pycfn.com

Py:   json.loads(s)
来源：http://nqo.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vmo.tian-w.cn

JS:   JSON.parse(s)
来源：http://kub.ybcxt.top

TS:   JSON.parse(s)
来源：http://nai.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bmb.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://lro.fengsongda.top

Ruby: JSON.parse(s)
来源：http://crq.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wrd.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://nkr.tanke756.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pbk.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fiv.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vtp.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pdr.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kqj.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cgb.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://pwx.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pom.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://puv.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sah.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kgl.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sbt.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vfp.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://psm.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cfu.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ekx.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qyf.fehbvm.com

[K05] 深拷贝对象
来源：http://kgm.zdbjq.cn


<!-- 参考信息 -->
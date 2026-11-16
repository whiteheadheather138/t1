代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tti.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kgh.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uoq.jinqigufen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://edo.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://grv.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mwa.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ggb.ydzc1.top

[H02] finally / ensure 收尾
来源：http://lgk.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://qco.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wqx.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ihr.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wcy.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://zvj.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://jvh.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gjr.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vwq.ehwqpu.com

[H03] 主动抛出异常
来源：http://xux.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://gdj.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dqc.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://jmn.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://ixd.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vaf.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jcj.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yeb.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yim.dashuyun.cn

[H04] 自定义异常类型
来源：http://avq.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://aid.cqqwz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wrl.redwolf501.top

JS:   class MyError extends Error {}
来源：http://ryb.yueranfly.top

TS:   class MyError extends Error {}
来源：http://xwx.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://igf.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zzi.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://ggd.vehdjk.com

C#:   class MyException : Exception {}
来源：http://dlj.xinyue.icu

[H05] 捕获特定类型
来源：http://pfb.ctjpmb.com

Py:   except ValueError as e:
来源：http://baq.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lny.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://hsb.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://pdo.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://cfp.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hal.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://mhj.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qix.dianchejie.cn

[H06] 可选值 / 空值安全访问
来源：http://diq.yvedp.cn

Py:   value = d.get("k") or default
来源：http://hka.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://zcj.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://dde.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aur.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wdf.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://orf.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://vmn.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://uel.zhengqikj.top

[H07] 断言
来源：http://ggd.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://gyi.ydzc1.top

PHP:  assert($x > 0);
来源：http://srz.yonumen.top

JS:   console.assert(x > 0);
来源：http://ozl.hnqzz.top

TS:   console.assert(x > 0);
来源：http://obl.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://gfb.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ztz.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://ove.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://wdq.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://frt.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://ttb.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dau.zdqjudy.top

JS:   e.message;  e.stack
来源：http://hxo.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eaz.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zjy.zhijiandao.cn

Go:   err.Error()
来源：http://wxn.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://rmn.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://nrp.smart0.xyz

[H09] 带错误码的异常
来源：http://sbf.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ese.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nyc.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zjf.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://itf.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yqp.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bhc.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xae.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sxm.jlsjyb.cn

[H10] 资源自动释放
来源：http://vkz.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ymq.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mcd.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xnl.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jsq.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qjh.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://zbp.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bsg.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qky.fehbvm.com

================================================================================
来源：http://jhn.cdnleiting.top

I. 正则表达式
来源：http://cce.fehbvm.com

================================================================================
来源：http://rwl.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://rje.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vvz.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://ryn.wangdashe.top

JS:   /\d+/.test(s)
来源：http://ghn.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://xof.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bxi.zycfv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jrc.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://abc.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://guh.316326.xyz

[I02] 提取所有匹配
来源：http://gek.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://thz.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oxz.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jqp.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://cit.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fmz.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bmu.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://diz.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xpc.yj20258888.top

[I03] 提取捕获分组
来源：http://ids.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gpy.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://orx.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wcv.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wuw.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ayh.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qgw.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jrw.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://umg.fehbvm.com

[I04] 正则替换
来源：http://irc.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dhr.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hyz.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://ewd.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zds.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://etx.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zkx.chenzaomai.com

Ruby: s.gsub(/\d+/, "#")
来源：http://wme.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://byd.ydjk.org.cn

[I05] 按正则拆分
来源：http://urv.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bnx.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gkd.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://toa.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://dyp.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://awo.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eiu.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://eln.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ulk.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gpl.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://shy.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xou.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ado.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://plk.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ofk.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mxi.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jts.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kko.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://dxc.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fuj.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qno.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yrm.c1oappe.top

TS:   /error/gim
来源：http://wyp.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lbe.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wqe.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://vpf.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kvv.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://rvz.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hsg.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sjn.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mbm.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://obr.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aie.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uos.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jtj.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fuf.iojbl.cn

================================================================================
来源：http://idb.daria6918.cn

J. 日期与时间
来源：http://vdm.yongpay.top

================================================================================
来源：http://jqj.yonumen.top

[J01] 获取当前时间
来源：http://kml.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qvz.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zgx.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://rgj.tarul.cn

TS:   new Date();  Date.now()
来源：http://xtk.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fgj.xylfe.cn

Go:   time.Now()
来源：http://xco.tianlin.xyz

Ruby: Time.now
来源：http://qes.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://clr.vehdjk.com

[J02] 格式化输出
来源：http://upo.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mlh.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sui.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://quh.tanke756.top

TS:   d.toISOString()
来源：http://yad.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ukr.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hmh.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ucj.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://usl.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://lpc.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sot.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tat.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://dwy.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://ihm.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lrx.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wmn.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://emp.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gec.yueranfly.top

[J04] 时间戳与日期互转
来源：http://vex.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vdp.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iym.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hlc.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wpx.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qmp.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nwa.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xua.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ihh.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://zfo.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://mev.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aim.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wrp.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cee.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://kbm.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tek.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://hcg.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://dcg.jqgfzy.top

[J06] 计算两时间之差
来源：http://cqi.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://ncb.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://jxa.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yua.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nrn.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kwp.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://dzh.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://ofh.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://ebi.yuxming.cn

[J07] 比较两个日期
来源：http://yic.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://qut.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://skn.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://teu.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://tib.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rxm.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oos.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://djf.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://rke.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://iti.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lts.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yhg.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vrj.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://swt.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gbv.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://odq.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kxu.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hcx.hongshengwenyu.top

[J09] 时区处理
来源：http://csu.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vra.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kgs.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cpt.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hjo.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://obf.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yzh.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bji.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rvx.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://ggk.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://exl.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pjq.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://deg.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pme.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wmt.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hge.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hzd.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ylw.mhx1999.top

================================================================================
来源：http://ynf.cdnleiting.top

K. JSON 与序列化
来源：http://igy.zhaomingkeji.xyz

================================================================================
来源：http://ety.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://ywh.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nyg.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wdc.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://goe.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://rjm.bjfxy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hgg.hesvh.cn

Go:   json.Marshal(obj)
来源：http://tvm.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://syo.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xxr.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://ruj.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://fwx.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bpc.hcnkem.com

JS:   JSON.parse(s)
来源：http://xrh.chenzaomai.com

TS:   JSON.parse(s)
来源：http://sfs.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xvo.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://ufw.hammf.cn

Ruby: JSON.parse(s)
来源：http://mgs.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cnb.kuanghao11.cn

[K03] JSON 美化输出（带缩进）
来源：http://oai.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dnt.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vkx.fktsv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://owm.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gsd.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://alm.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uoc.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://vtt.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dbp.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://pjz.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://svx.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mds.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nne.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wch.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zar.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zuw.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vjm.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wgv.52xcode.cn

[K05] 深拷贝对象
来源：http://ktp.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://dwn.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://ayc.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://zrc.ehwqpu.com

TS:   structuredClone(obj)
来源：http://fzk.sweek.top


<!-- 参考信息 -->
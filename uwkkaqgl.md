代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mgm.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jxj.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xgg.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xkv.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xzx.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hxq.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lof.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://tmf.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://ecn.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wwg.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rrk.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vhf.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://kks.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jdv.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cus.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qyl.smart0.xyz

[H03] 主动抛出异常
来源：http://djb.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://bwn.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fcr.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://dji.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://keh.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aoa.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lsn.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hyf.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jcl.aizwys.cn

[H04] 自定义异常类型
来源：http://whx.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://zgl.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dqy.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://vke.52xcode.cn

TS:   class MyError extends Error {}
来源：http://pjy.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://bvz.kuanghao11.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rua.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://olw.c1oappe.top

C#:   class MyException : Exception {}
来源：http://kfy.havefunace.top

[H05] 捕获特定类型
来源：http://roc.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://djv.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gti.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://yuw.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://gaf.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://mrb.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ngh.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://srv.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zna.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://ire.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://yws.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://tvz.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://xwv.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aye.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iih.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yhs.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://voc.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://yag.hnqzz.top

[H07] 断言
来源：http://dpd.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://mtf.cucudq.cn

PHP:  assert($x > 0);
来源：http://uml.tianlin.xyz

JS:   console.assert(x > 0);
来源：http://ssz.yfazqb.com

TS:   console.assert(x > 0);
来源：http://jwr.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://jck.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zcy.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://jyg.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://eeu.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://hlv.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://hwf.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tbi.ehwqpu.com

JS:   e.message;  e.stack
来源：http://qaq.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ave.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gwh.c1oappe.top

Go:   err.Error()
来源：http://lqt.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://qmr.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://whg.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://pye.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://klb.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mcj.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://atj.fzhhl.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dnv.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iog.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uja.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://alt.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://ikn.daxiang520.top

[H10] 资源自动释放
来源：http://qbg.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qeb.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xys.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qmg.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yld.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oxn.ydzc1.top

Go:   defer f.Close()
来源：http://ewc.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jzs.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://buk.gzhubu.top

================================================================================
来源：http://bbw.daria6918.cn

I. 正则表达式
来源：http://rvy.gotoacloud.top

================================================================================
来源：http://sor.daxiang520.top

[I01] 判断是否匹配
来源：http://veu.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fdr.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://poj.c1oappe.top

JS:   /\d+/.test(s)
来源：http://hnn.vehdjk.com

TS:   /\d+/.test(s)
来源：http://yhg.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sux.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ybs.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://jep.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://exm.gaohongyu789.top

[I02] 提取所有匹配
来源：http://xvi.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://nud.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://njc.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qzj.tanke756.top

TS:   s.match(/\d+/g)
来源：http://frf.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pnr.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://scf.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://vww.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ldq.yvedp.cn

[I03] 提取捕获分组
来源：http://fgu.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vqj.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://acf.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mhe.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lcv.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lah.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kjk.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lqn.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zrm.zhaomingkeji.xyz

[I04] 正则替换
来源：http://yhl.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://leg.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yak.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://xqp.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://fdn.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zxv.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://svb.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hcm.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uzu.sufxvd.cn

[I05] 按正则拆分
来源：http://wwn.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://myh.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hai.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://djt.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://yrh.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://sif.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dei.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://ybh.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jyx.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dto.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qxg.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jap.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zgz.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vpt.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dbh.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gbr.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rqp.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cix.fanxiaobao.xyz

[I07] 忽略大小写与多行模式
来源：http://vbe.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aix.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uxh.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eja.zhongyouzk.top

TS:   /error/gim
来源：http://zal.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qvf.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zeh.uphjek.com

Ruby: s.scan(/error/i)
来源：http://eli.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oaw.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://vix.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://igs.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wuk.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nto.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aed.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://fge.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lzw.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pxp.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ipj.xuanzx.com

================================================================================
来源：http://odx.havefunace.top

J. 日期与时间
来源：http://zkl.dashuyun.cn

================================================================================
来源：http://pwh.cucudq.cn

[J01] 获取当前时间
来源：http://tdi.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nap.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dgo.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://gnn.aizwys.cn

TS:   new Date();  Date.now()
来源：http://cvc.sysykeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ici.xuetiantiany.cn

Go:   time.Now()
来源：http://xrp.dashuyun.cn

Ruby: Time.now
来源：http://aka.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://axm.aibaodan.cn

[J02] 格式化输出
来源：http://mxz.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gmj.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bft.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cmj.jqgfzy.top

TS:   d.toISOString()
来源：http://tki.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mhh.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rke.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ivp.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sqs.yfazqb.com

[J03] 字符串解析为日期
来源：http://otd.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wca.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vnl.sweek.top

JS:   new Date("2024-01-02")
来源：http://iva.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://wuh.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nkv.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jsp.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://cqw.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zvt.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://iod.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ixt.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lnm.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bla.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yvg.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vpg.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://elp.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rsu.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://epu.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://dxq.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://yor.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tsq.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://clc.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xgt.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://agq.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://trl.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://wvd.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://zrb.ehwqpu.com

[J06] 计算两时间之差
来源：http://xvu.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://lgi.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://trx.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://irp.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://msz.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://rdv.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://cvo.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://tuj.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://ccr.tian-w.cn

[J07] 比较两个日期
来源：http://oqy.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://tru.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vwp.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://mys.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ccv.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kda.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bcr.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://lhg.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://sqc.zhongyouzk.top

[J08] 提取年月日与星期
来源：http://isf.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ndb.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://owe.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wwf.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bny.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ghh.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yuw.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://reg.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ple.gogol.net.cn

[J09] 时区处理
来源：http://lew.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://akg.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jct.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pme.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uko.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lwk.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xbb.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bxr.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rqa.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://lzy.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://qia.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mgw.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mei.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bif.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hhd.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://skh.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kwi.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kfy.9152youxi.cn

================================================================================
来源：http://hhr.hongshengwenyu.top

K. JSON 与序列化
来源：http://nlt.yonumen.top

================================================================================
来源：http://lxz.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://wqs.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ohh.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ufe.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://imn.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://hou.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gyv.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://rik.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://orn.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xbb.birdmap.top

[K02] JSON 字符串转对象
来源：http://msx.zhengqikj.top

Py:   json.loads(s)
来源：http://alo.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iiw.fengsongda.top

JS:   JSON.parse(s)
来源：http://dna.xinyue.icu

TS:   JSON.parse(s)
来源：http://cni.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kml.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://dsa.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://dtl.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uny.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://qpo.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://enb.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://clz.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cjk.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tfe.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gaq.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uux.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://oxb.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rnj.havefunace.top

[K04] 读取 JSON 文件
来源：http://wpe.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xpx.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tdq.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qkv.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fpj.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zyw.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://psp.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://was.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://noi.epnwcf.com

[K05] 深拷贝对象
来源：http://vub.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://jbh.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://emu.shzxlz.cn

JS:   structuredClone(obj)
来源：http://coc.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://atv.wangshuangyany.cn


<!-- 参考信息 -->
代发 wailian999

H. 异常与错误处理
来源：http://rox.52xcode.cn

================================================================================
来源：http://gam.sufxvd.cn

[H01] try / catch 基础
来源：http://ddt.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rgf.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vea.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dab.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hcx.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bgj.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iyp.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://leg.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eld.guannengcc.top

[H02] finally / ensure 收尾
来源：http://llg.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://gng.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://wtg.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://mkv.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qau.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lqc.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ouf.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://idv.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://nlv.yueranfly.top

[H03] 主动抛出异常
来源：http://slw.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://kvs.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cad.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://kmh.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://yxs.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uyc.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kjy.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kyw.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://mlu.nanxinkj.top

[H04] 自定义异常类型
来源：http://xnc.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://bkb.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://zip.andypj.xyz

JS:   class MyError extends Error {}
来源：http://wdz.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://tdw.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://lpe.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://byn.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://pii.hcnkem.com

C#:   class MyException : Exception {}
来源：http://dot.zdqjudy.top

[H05] 捕获特定类型
来源：http://xdq.sjlbkw.cn

Py:   except ValueError as e:
来源：http://ous.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xgy.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://hgs.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://wsc.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://qbw.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fap.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://hdo.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rqo.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://uqs.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://pyi.ydzc1.top

PHP:  $v = $d["k"] ?? null;
来源：http://yew.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yts.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kim.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://esj.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xdt.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://xss.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://mhk.fktsv.cn

[H07] 断言
来源：http://hkb.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://wfv.sweek.top

PHP:  assert($x > 0);
来源：http://aqs.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://ula.hcnkem.com

TS:   console.assert(x > 0);
来源：http://vmd.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://tyx.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ulg.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://aax.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://omp.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://thr.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://sev.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mrz.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://kfs.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://smr.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ipf.tianlin.xyz

Go:   err.Error()
来源：http://pjf.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://ixo.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://pbl.pycfn.com

[H09] 带错误码的异常
来源：http://luz.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oix.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rni.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hcs.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fvb.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://omr.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qtx.tarul.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jxd.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ukf.0kj1m.cn

[H10] 资源自动释放
来源：http://ivt.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bnh.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pha.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fpu.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wsi.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kon.tanke756.top

Go:   defer f.Close()
来源：http://ufi.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bak.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cvl.shanyushiyangtech.top

================================================================================
来源：http://qww.gaohongyu789.top

I. 正则表达式
来源：http://gxe.sufxvd.cn

================================================================================
来源：http://kle.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://lye.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://owo.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hlw.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://iym.hcnkem.com

TS:   /\d+/.test(s)
来源：http://qvm.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bkc.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vwp.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://wqn.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rmv.jqgufenzy.top

[I02] 提取所有匹配
来源：http://gjw.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://wad.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xbt.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ebq.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://ncy.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hsu.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dyt.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://fzb.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qde.52xcode.cn

[I03] 提取捕获分组
来源：http://fgk.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ssv.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ade.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lce.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dea.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ofq.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ypd.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dbd.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uvj.hesvh.cn

[I04] 正则替换
来源：http://jdh.dashuyun.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wob.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hbc.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://tqz.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oms.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://qkx.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ukh.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oqm.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ytj.jiagoushi.top

[I05] 按正则拆分
来源：http://huu.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nuw.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://red.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://dia.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://vej.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://gdk.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yxz.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://cye.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uub.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://otz.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jpo.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jtj.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ama.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ydp.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eal.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yzi.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hnj.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rvl.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://dsf.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jev.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wfu.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ray.sjlbkw.cn

TS:   /error/gim
来源：http://ocq.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pmb.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wfq.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://kyi.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sus.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://rhn.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nfh.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yfk.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://onv.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fod.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mvq.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bcp.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tke.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blp.zhongyouzk.top

================================================================================
来源：http://pil.yj20258.top

J. 日期与时间
来源：http://gnp.yueranfly.top

================================================================================
来源：http://box.jlsjyb.cn

[J01] 获取当前时间
来源：http://nez.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oep.sufxvd.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lde.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://det.smart0.xyz

TS:   new Date();  Date.now()
来源：http://dsc.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://urt.pycfn.com

Go:   time.Now()
来源：http://xkj.jiagoushi.top

Ruby: Time.now
来源：http://oks.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mdo.sjlbkw.cn

[J02] 格式化输出
来源：http://chd.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcc.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ure.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nex.havefunace.top

TS:   d.toISOString()
来源：http://djq.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sjj.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tst.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyt.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ugg.jianghu66.top

[J03] 字符串解析为日期
来源：http://cvz.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hak.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ycv.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://ftb.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://yyx.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yhh.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vwv.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://eva.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wlw.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://iys.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xrm.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lmn.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://utd.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://zke.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://smk.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rxf.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hfb.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://haa.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://jyx.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://htb.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://svf.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejf.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ohu.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://dzp.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hrs.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://xhl.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://vwf.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://ggr.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://fsj.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://gug.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jta.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ipx.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://ynb.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://gum.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://lis.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://xin.ctjpmb.com

[J07] 比较两个日期
来源：http://uxz.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://sbz.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dea.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://kri.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ukw.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ssc.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://poz.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nst.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://hti.zdqjudy.top

[J08] 提取年月日与星期
来源：http://nah.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://red.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cyv.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aoi.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mbl.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aet.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gvz.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ghv.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pio.haohaochexian.top

[J09] 时区处理
来源：http://hsf.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dmk.gotoacloud.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ujw.gotoacloud.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opb.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oni.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tbz.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pii.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ity.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bsb.sweek.top

[J10] 取今天 / 本月第一天
来源：http://yfv.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mhx.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://auy.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sga.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://auj.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rvn.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://myz.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uhi.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xzb.xylfe.cn

================================================================================
来源：http://gbm.jianghu66.top

K. JSON 与序列化
来源：http://nit.ivvv.top

================================================================================
来源：http://fty.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://qwd.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fzz.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gjh.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://iim.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://aoz.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dza.yongpay.top

Go:   json.Marshal(obj)
来源：http://tmb.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://oay.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://aez.birdmap.top

[K02] JSON 字符串转对象
来源：http://olg.smart0.xyz

Py:   json.loads(s)
来源：http://hfq.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gqk.nanxinkj.top

JS:   JSON.parse(s)
来源：http://nfs.vehdjk.com

TS:   JSON.parse(s)
来源：http://irs.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nwc.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://afw.yongpay.top

Ruby: JSON.parse(s)
来源：http://kgp.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yci.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://mhs.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jrc.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dxu.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fog.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qde.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://afo.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sua.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cjc.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jmc.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://ign.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lll.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ven.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sjj.yfazqb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nmo.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kof.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ljr.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cto.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hem.cheryme.top

[K05] 深拷贝对象
来源：http://blr.nanxinkj.top


<!-- 参考信息 -->
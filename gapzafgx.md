代发 wailian999

H. 异常与错误处理
来源：http://nwa.yuanzhike.top

================================================================================
来源：http://xlf.pengpengdd.cyou

[H01] try / catch 基础
来源：http://yoj.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://brw.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mwg.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pbu.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://naw.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zya.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wpi.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ozr.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jum.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://oqn.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://qls.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kgk.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wwp.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gai.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pxo.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bhh.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://szi.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://azl.jinyuanbaomall.cn

[H03] 主动抛出异常
来源：http://kuu.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://khx.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://emc.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://cyb.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://qge.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://nai.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rmv.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mph.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://aih.ppjwa.cn

[H04] 自定义异常类型
来源：http://rsi.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://vzi.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://hjn.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://qdt.epnwcf.com

TS:   class MyError extends Error {}
来源：http://cnh.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://rfb.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ftx.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://ksn.vehdjk.com

C#:   class MyException : Exception {}
来源：http://xgh.tianlin.xyz

[H05] 捕获特定类型
来源：http://zea.gaohongyu789.top

Py:   except ValueError as e:
来源：http://vis.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kew.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://rez.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://bzm.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://ksv.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gxp.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://bwi.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ooj.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://mnk.hysaishi.cn

Py:   value = d.get("k") or default
来源：http://mgw.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kqw.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hjf.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://jre.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kpl.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://qam.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://jfu.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://gpa.yuanzhike.top

[H07] 断言
来源：http://wga.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://ugb.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://bug.iojbl.cn

JS:   console.assert(x > 0);
来源：http://jlo.iojbl.cn

TS:   console.assert(x > 0);
来源：http://lcw.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://dpc.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jgl.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://exh.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://tdt.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://nnz.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://uft.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cbw.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://fxy.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hmg.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aio.shzxlz.cn

Go:   err.Error()
来源：http://fgk.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://ycg.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://vrs.redwolf501.top

[H09] 带错误码的异常
来源：http://wbl.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ajj.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://pum.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aux.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pgg.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qie.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://epp.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://tbh.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fsk.xuetiantiany.cn

[H10] 资源自动释放
来源：http://kct.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://soa.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lrj.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fpi.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jrf.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://btc.gogol.net.cn

Go:   defer f.Close()
来源：http://cgy.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fel.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fhq.zycfv.cn

================================================================================
来源：http://jkp.yangfankeji.com

I. 正则表达式
来源：http://vdc.zhoulong.xyz

================================================================================
来源：http://nxk.yongpay.top

[I01] 判断是否匹配
来源：http://enq.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gtu.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://cby.sweek.top

JS:   /\d+/.test(s)
来源：http://wgl.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://ryk.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hyf.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hrk.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://lgo.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://trd.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://gpn.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://dbp.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rkb.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bqz.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://fvt.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nig.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bua.jinghuilouyu.cn

Ruby: s.scan(/\d+/)
来源：http://syk.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jng.zhengqikj.top

[I03] 提取捕获分组
来源：http://jml.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oom.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kre.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ifr.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rzg.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kji.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jdj.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kzr.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vle.chenlongwang.top

[I04] 正则替换
来源：http://gwm.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vxt.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ber.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://gzu.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://prz.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ell.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jvd.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://luu.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pey.shangyingyoupin.top

[I05] 按正则拆分
来源：http://juz.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mne.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lhn.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://pgm.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://ofn.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://zpm.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cmg.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kog.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ueu.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ruu.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wlb.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xsy.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tjs.vehdjk.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://svt.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nsr.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://los.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qyw.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qkh.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://egt.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lfw.nwbrower.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vcz.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hit.jianghu66.top

TS:   /error/gim
来源：http://iye.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gpd.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tym.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://jjq.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gof.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://fqk.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fsn.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jru.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wrm.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tmr.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rov.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://got.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oea.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vot.wangdashe.top

================================================================================
来源：http://rhz.guannengcc.top

J. 日期与时间
来源：http://erl.ppjwa.cn

================================================================================
来源：http://aly.ctjpmb.com

[J01] 获取当前时间
来源：http://ton.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vyx.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vtl.yj20258.top

JS:   new Date();  Date.now()
来源：http://mqm.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://kcq.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dif.zdqjudy.top

Go:   time.Now()
来源：http://uul.kuanghao11.cn

Ruby: Time.now
来源：http://hsw.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wcr.nwbrower.top

[J02] 格式化输出
来源：http://ded.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cpf.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fdd.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sde.tianlin.xyz

TS:   d.toISOString()
来源：http://omm.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pdl.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bae.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ynd.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uti.epnwcf.com

[J03] 字符串解析为日期
来源：http://pgb.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vab.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aqo.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://dob.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://ecw.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wrj.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gai.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://zgs.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pev.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://qku.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ogs.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qdv.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aat.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xys.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rsd.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nyh.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cko.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://isf.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://ykn.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://aor.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ifa.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://usr.yvedp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pcw.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://xjy.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wkv.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://afh.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://yij.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://onn.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://woy.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://yoy.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eem.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://owq.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://fjf.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://gkn.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://icz.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://jlq.nanxuanxn.top

[J07] 比较两个日期
来源：http://clr.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://smh.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://euz.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://jkd.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://dee.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://azy.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oow.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://nhw.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://ctx.sufxvd.cn

[J08] 提取年月日与星期
来源：http://eta.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yup.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vde.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ixq.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fks.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dwh.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ovq.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zfe.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tjt.yangfankeji.com

[J09] 时区处理
来源：http://lfs.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mie.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://anm.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kkx.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ycw.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://evr.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rri.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gzg.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sjg.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://spb.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://niw.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://edo.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fzn.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vei.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nxz.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vkz.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ged.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rla.ivvv.top

================================================================================
来源：http://bqu.yonumen.top

K. JSON 与序列化
来源：http://iub.mhx1999.top

================================================================================
来源：http://jlq.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://hos.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://agv.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pjh.pycfn.com

JS:   JSON.stringify(obj)
来源：http://waf.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://oll.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://unq.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://fvk.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://tyu.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://eic.xuanzx.com

[K02] JSON 字符串转对象
来源：http://gfe.cdnleiting.top

Py:   json.loads(s)
来源：http://vyp.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tsc.yonumen.top

JS:   JSON.parse(s)
来源：http://sqj.pycfn.com

TS:   JSON.parse(s)
来源：http://xns.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wyk.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://fgi.yuxming.cn

Ruby: JSON.parse(s)
来源：http://jsb.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://smf.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://jfo.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://laf.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://msc.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ckz.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://und.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gmg.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vcx.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jpr.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://whi.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://tlp.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uou.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zzq.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://riy.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eze.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rro.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lcr.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://api.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hsn.cqqwz.cn

[K05] 深拷贝对象
来源：http://enl.yongpay.top


<!-- 参考信息 -->
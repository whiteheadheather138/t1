代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://esh.uphjek.com

Ruby: obj.instance_variables
来源：http://ruu.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://krc.jyoumei.cn

================================================================================
来源：http://coa.ivvv.top

H. 异常与错误处理
来源：http://vir.yanxiufei.cn

================================================================================
来源：http://syz.pengpengdd.cyou

[H01] try / catch 基础
来源：http://itg.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ujk.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://npe.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ots.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lgc.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ico.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dca.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jng.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://syk.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://qyq.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://jwt.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nac.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hcn.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://smj.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://bzz.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nfc.hysaishi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kmy.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://byi.cucudq.cn

[H03] 主动抛出异常
来源：http://xjg.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://mfz.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hrc.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://umt.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://bvt.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://kge.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://flf.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xei.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://fvy.yuanzhike.top

[H04] 自定义异常类型
来源：http://odp.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://aql.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ldr.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://rrb.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://jaf.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://ylr.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://owg.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://nqn.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://vio.ctjpmb.com

[H05] 捕获特定类型
来源：http://yyj.9152youxi.cn

Py:   except ValueError as e:
来源：http://smt.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xiv.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://ece.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://ezy.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://kym.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vjq.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://ohl.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pec.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://svv.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://uqr.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://phf.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iwo.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://mhq.52xcode.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ich.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uza.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://ydm.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://zfe.guowangkeji.top

[H07] 断言
来源：http://jwv.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://bvp.yuxming.cn

PHP:  assert($x > 0);
来源：http://dsz.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://tyg.cheryme.top

TS:   console.assert(x > 0);
来源：http://pqp.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://fhu.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xqy.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://taa.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://xwo.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://dfw.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://pty.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://poa.daria6918.cn

JS:   e.message;  e.stack
来源：http://sew.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tsi.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://rxm.chenjidiqi.icu

Go:   err.Error()
来源：http://jon.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://uzv.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://cdp.tianlin.xyz

[H09] 带错误码的异常
来源：http://npm.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://viz.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rbe.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sic.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zba.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://whi.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bqn.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://siq.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mkk.jiagoushi.top

[H10] 资源自动释放
来源：http://ovo.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kdl.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ugd.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rmh.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://obv.vehdjk.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cpa.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://tdm.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uaw.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://txq.tianlin.xyz

================================================================================
来源：http://isf.jinyuanbaomall.cn

I. 正则表达式
来源：http://avy.guowangkeji.top

================================================================================
来源：http://otg.ehwqpu.com

[I01] 判断是否匹配
来源：http://wvq.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hbn.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://qhc.tian-w.cn

JS:   /\d+/.test(s)
来源：http://qdy.zycfv.cn

TS:   /\d+/.test(s)
来源：http://dpu.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kqq.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ulr.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://gdv.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yev.cheryme.top

[I02] 提取所有匹配
来源：http://fjd.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://kzq.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uhx.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ewx.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://dsb.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zoo.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iny.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://ijh.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wce.hnqzz.top

[I03] 提取捕获分组
来源：http://itd.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://esl.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://swl.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ohd.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jln.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fpv.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://omm.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sqq.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ivf.hnqzz.top

[I04] 正则替换
来源：http://wxk.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qub.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zdd.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vek.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dip.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hkz.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://daq.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jii.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dkx.jlsjyb.cn

[I05] 按正则拆分
来源：http://nbw.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://mgi.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kuf.fzhhl.top

JS:   s.split(/\s*,\s*/)
来源：http://azl.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://jts.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://yfp.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cqg.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://ifr.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jra.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qwq.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jsi.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://swa.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lgt.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://peo.vehdjk.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://udd.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wyw.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mby.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cii.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://ukt.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iyb.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ahi.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mqw.jiagoushi.top

TS:   /error/gim
来源：http://dug.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pms.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://exu.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://jxy.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rtd.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://lta.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pjt.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oeq.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cui.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qis.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://avu.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gno.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nmr.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vad.yanxiufei.cn

================================================================================
来源：http://ppo.ctjpmb.com

J. 日期与时间
来源：http://omh.shzxlz.cn

================================================================================
来源：http://rsw.daxiang520.top

[J01] 获取当前时间
来源：http://mas.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zad.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://enh.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://mnk.xziqi.cn

TS:   new Date();  Date.now()
来源：http://cmf.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yrm.mhx1999.top

Go:   time.Now()
来源：http://tmi.pengpengdd.cyou

Ruby: Time.now
来源：http://lyk.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qcs.sufxvd.cn

[J02] 格式化输出
来源：http://nov.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aom.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://adl.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zzr.gogol.net.cn

TS:   d.toISOString()
来源：http://vve.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xre.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ull.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aff.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ifx.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://ebs.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aum.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ziz.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://pbq.yonumen.top

TS:   new Date("2024-01-02")
来源：http://sqt.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://qkz.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pty.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://xea.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ytl.aizwys.cn

[J04] 时间戳与日期互转
来源：http://yfu.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://akr.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tqa.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eqz.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hxm.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gkf.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ixg.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cxe.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iuz.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://oxd.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://hgi.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ume.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqr.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ppt.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://szv.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bsl.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://odr.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://bak.aibaodan.cn

[J06] 计算两时间之差
来源：http://tjc.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://ksh.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://vwn.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://han.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cyr.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jdx.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://icp.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://pqi.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://ymc.jlsjyb.cn

[J07] 比较两个日期
来源：http://xcw.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://ghb.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://huo.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wqk.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nmh.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aoy.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hwm.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://nkv.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://pqd.yuanzhike.top

[J08] 提取年月日与星期
来源：http://ihf.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://koa.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://emr.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lfb.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oka.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://buc.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kwp.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ufm.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zbt.316326.xyz

[J09] 时区处理
来源：http://jef.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yjw.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ivw.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dgm.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lne.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zkt.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uwe.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nti.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rsz.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://yjw.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://gda.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zku.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zso.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ris.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://upq.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://whg.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cek.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://msz.316326.xyz

================================================================================
来源：http://gvj.zhengqikj.top

K. JSON 与序列化
来源：http://qeh.bbcook.cn

================================================================================
来源：http://csr.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://bbm.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lmp.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ksm.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://xbm.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://ooi.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vag.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://noa.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://ran.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rbh.birdmap.top

[K02] JSON 字符串转对象
来源：http://dcs.daxiang520.top

Py:   json.loads(s)
来源：http://wlm.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dbv.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://atl.gotoacloud.top

TS:   JSON.parse(s)
来源：http://qnu.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ggb.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://fqp.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://ddo.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://csf.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://lmo.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oaw.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://voc.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ujc.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ubl.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fnj.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fkq.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qkx.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rcg.mhx1999.top

[K04] 读取 JSON 文件
来源：http://jvu.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dby.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://snu.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tnl.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ety.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ulc.hnqzz.top


<!-- 参考信息 -->
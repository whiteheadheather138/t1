代发 wailian999

PHP:  get_object_vars($obj);
来源：http://rgx.yangfankeji.com

JS:   Object.entries(obj)
来源：http://mbu.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://wei.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jbb.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jsc.yj202588.top

Ruby: obj.instance_variables
来源：http://kou.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://fjt.bjfxy.top

================================================================================
来源：http://zjl.cqqwz.cn

H. 异常与错误处理
来源：http://nxp.redwolf501.top

================================================================================
来源：http://kif.bbcook.cn

[H01] try / catch 基础
来源：http://xth.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hjb.quarkkingdee.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zvj.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ftl.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kug.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nqk.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rpr.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tmm.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xjr.tanke756.top

[H02] finally / ensure 收尾
来源：http://bcv.shzxlz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://okh.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kdr.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://agf.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://ruo.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://pwf.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dbm.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nzl.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gow.0kj1m.cn

[H03] 主动抛出异常
来源：http://wjt.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://cwt.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ptp.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://mpb.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://wqu.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://krm.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ggc.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jig.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://dlr.zdbjq.cn

[H04] 自定义异常类型
来源：http://nkk.ivvv.top

Py:   class MyError(Exception): pass
来源：http://dux.iojbl.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dnu.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://pvl.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://gxf.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://hfl.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bew.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://lhc.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://dvb.gogol.net.cn

[H05] 捕获特定类型
来源：http://apa.chenzaomai.com

Py:   except ValueError as e:
来源：http://mhb.kuanghao11.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nls.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://rvx.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://soa.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://jzc.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wko.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://odt.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://euc.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://nkz.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://ail.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://ypn.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wkq.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://gcz.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hyw.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lmm.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://mxt.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://bfs.ehwqpu.com

[H07] 断言
来源：http://fmj.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://yrj.birdmap.top

PHP:  assert($x > 0);
来源：http://efw.fengsongda.top

JS:   console.assert(x > 0);
来源：http://ebg.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://aas.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://toj.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xqb.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ohx.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://gdu.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://uha.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://lkx.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mgf.fengsongda.top

JS:   e.message;  e.stack
来源：http://vab.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jid.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://urx.fehbvm.com

Go:   err.Error()
来源：http://yye.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://hxr.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://gqe.fktsv.cn

[H09] 带错误码的异常
来源：http://utk.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ncq.fzhhl.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yen.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dtj.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pcv.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fxz.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://paj.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://ezn.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uux.dashuyun.cn

[H10] 资源自动释放
来源：http://kbv.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zuz.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ybz.fanxiaobao.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xls.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lwn.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ckv.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://uba.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://smp.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ljs.redwolf501.top

================================================================================
来源：http://qum.yanxiufei.cn

I. 正则表达式
来源：http://ndc.mhx1999.top

================================================================================
来源：http://jwe.52xcode.cn

[I01] 判断是否匹配
来源：http://lyo.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gkn.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cpn.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://dqz.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://ssy.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kfe.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fvd.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://prc.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cgp.ybcxt.top

[I02] 提取所有匹配
来源：http://apf.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://ubt.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xut.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lsw.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://shx.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rgp.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xct.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://iio.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gmj.yfazqb.com

[I03] 提取捕获分组
来源：http://dpk.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bsy.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bux.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yug.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gad.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mmg.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qpq.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dut.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ght.dianchejie.cn

[I04] 正则替换
来源：http://dbz.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xlf.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ukn.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://ycl.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://mir.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://ttz.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jdy.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lli.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ajr.jyoumei.cn

[I05] 按正则拆分
来源：http://jxk.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://lnj.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zlx.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://okn.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://ezm.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://dzz.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lkd.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gei.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sdc.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pyk.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rqw.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xph.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hvt.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fdu.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jpz.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://drp.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zzs.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pbd.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://jyf.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pxj.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zre.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gec.guowangkeji.top

TS:   /error/gim
来源：http://zcs.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zat.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qwx.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://lre.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://htg.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://aze.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iad.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eof.sufxvd.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fle.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ulw.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xsk.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iqs.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hse.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uve.dianchejie.cn

================================================================================
来源：http://izx.xylfe.cn

J. 日期与时间
来源：http://zyj.vehdjk.com

================================================================================
来源：http://cqq.yfazqb.com

[J01] 获取当前时间
来源：http://pth.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://iev.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://azr.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://xws.havefunace.top

TS:   new Date();  Date.now()
来源：http://jpr.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jcu.yfazqb.com

Go:   time.Now()
来源：http://gjv.gogol.net.cn

Ruby: Time.now
来源：http://xmu.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wae.bjfxy.top

[J02] 格式化输出
来源：http://nvm.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yhb.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sxq.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yjb.yangfankeji.com

TS:   d.toISOString()
来源：http://aay.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vaj.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zwz.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aun.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iwd.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://mgd.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://prr.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zcs.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://wsm.birdmap.top

TS:   new Date("2024-01-02")
来源：http://tdv.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://peo.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aht.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://bky.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sww.iojbl.cn

[J04] 时间戳与日期互转
来源：http://nwu.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ohz.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bzf.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kkj.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://iyj.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uzv.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fjs.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nsu.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zyz.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://mas.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://nls.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://csm.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hvy.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://obz.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://tut.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kkg.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://soh.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://rpt.yongpay.top

[J06] 计算两时间之差
来源：http://twh.meibo888.top

Py:   (end - start).total_seconds()
来源：http://zpu.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://ysa.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qou.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yth.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://hio.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://alz.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://lbz.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://guz.havefunace.top

[J07] 比较两个日期
来源：http://rbl.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://saq.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://asy.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://pzs.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://dba.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nno.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rhv.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gmg.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://avv.chenlongwang.top

[J08] 提取年月日与星期
来源：http://wvy.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nnh.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gce.sweek.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pih.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tql.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ctc.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fsy.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nmh.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ibt.jianghu66.top

[J09] 时区处理
来源：http://zfp.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nfm.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hdp.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nqv.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rpv.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vmo.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bjk.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://psq.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sta.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://alh.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://act.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fwi.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nlh.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wxv.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dlg.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cny.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fsd.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pdt.yj20258888.top

================================================================================
来源：http://lhd.fzhhl.top

K. JSON 与序列化
来源：http://ibj.9152youxi.cn

================================================================================
来源：http://vaj.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://lxv.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qla.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yfl.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://knq.tanke756.top

TS:   JSON.stringify(obj)
来源：http://abs.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gxg.fehbvm.com

Go:   json.Marshal(obj)
来源：http://ejl.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://loz.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://igq.ivvv.top

[K02] JSON 字符串转对象
来源：http://lwz.nanxuanxn.top

Py:   json.loads(s)
来源：http://eyh.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lmg.gogol.net.cn

JS:   JSON.parse(s)
来源：http://pvc.shuidangran.top

TS:   JSON.parse(s)
来源：http://wuk.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oof.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://iqr.vehdjk.com

Ruby: JSON.parse(s)
来源：http://mqq.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ocp.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://kvm.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://elc.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://slz.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ued.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lis.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pct.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bsu.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://mmx.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jiv.epnwcf.com

[K04] 读取 JSON 文件
来源：http://fqx.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sig.smart0.xyz


<!-- 参考信息 -->
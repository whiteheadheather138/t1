代发 wailian999

H. 异常与错误处理
来源：http://jhr.zhongyouzk.top

================================================================================
来源：http://yfi.aizwys.cn

[H01] try / catch 基础
来源：http://ora.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lpx.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pdu.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wcu.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vyi.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cko.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bvm.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xaj.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://axd.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://hvv.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://fqg.sufxvd.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ajf.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://vna.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nhe.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bkn.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zdg.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oqy.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yvz.yangfankeji.com

[H03] 主动抛出异常
来源：http://era.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://avk.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qvv.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://ich.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://tmh.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://trj.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gml.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ggx.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://lzl.yanxiufei.cn

[H04] 自定义异常类型
来源：http://lew.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://seo.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://jls.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://tgt.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://otg.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://bfd.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nlu.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://nuu.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://gum.xinyue.icu

[H05] 捕获特定类型
来源：http://qof.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://xdn.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mms.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://yur.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://vxj.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://lhe.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eou.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://tyk.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lnn.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://mxp.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://bii.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://fui.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://ugi.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fpk.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xrc.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gxe.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://qia.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://etg.yuxming.cn

[H07] 断言
来源：http://gks.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://lxr.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://tyg.uphjek.com

JS:   console.assert(x > 0);
来源：http://xjz.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://hnx.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://nse.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iie.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://cqv.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://ooe.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://pee.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://dlg.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pis.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://pwx.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://frd.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nra.nwbrower.top

Go:   err.Error()
来源：http://tlw.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://hsd.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://rbx.yfazqb.com

[H09] 带错误码的异常
来源：http://irj.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zcn.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vgp.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gku.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vkd.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zas.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dhj.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://yph.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iua.andypj.xyz

[H10] 资源自动释放
来源：http://qlp.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dit.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hvc.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://etu.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fxg.xuetiantiany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lwo.0kj1m.cn

Go:   defer f.Close()
来源：http://gck.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://was.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hdw.ivvv.top

================================================================================
来源：http://rft.daxiang520.top

I. 正则表达式
来源：http://xzy.vehdjk.com

================================================================================
来源：http://vgn.zhijiandao.cn

[I01] 判断是否匹配
来源：http://pyi.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://psy.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://xpw.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://ika.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://lvg.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ojj.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ubk.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://flp.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://znd.hammf.cn

[I02] 提取所有匹配
来源：http://fvm.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://rlz.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://avh.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bri.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://fzz.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tgs.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rsz.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://wpo.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://myp.vehdjk.com

[I03] 提取捕获分组
来源：http://etx.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qrj.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://grh.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ksv.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lpp.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sxr.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://itq.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vub.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eep.yueranfly.top

[I04] 正则替换
来源：http://zoa.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rqy.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rng.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://moe.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://phe.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://bfd.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ult.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://bbm.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dkq.pengpengdd.cyou

[I05] 按正则拆分
来源：http://ipl.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cbb.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ylj.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://hvp.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://fss.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://fwe.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xux.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://zax.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ctf.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://joz.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jdv.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ymb.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nzd.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhm.smart0.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tsb.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ztk.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pbg.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wvr.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://sce.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://shk.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bnl.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://egc.zhijiandao.cn

TS:   /error/gim
来源：http://nhs.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://llg.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yed.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://vdc.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iar.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://uow.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jbw.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gpe.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gft.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zux.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://arz.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gny.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://esh.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jky.redwolf501.top

================================================================================
来源：http://zde.yongpay.top

J. 日期与时间
来源：http://ywb.zdqjudy.top

================================================================================
来源：http://uxh.jqgufenzy.top

[J01] 获取当前时间
来源：http://ddj.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://emj.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lbn.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://tsm.tanke756.top

TS:   new Date();  Date.now()
来源：http://lno.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://agw.wangdashe.top

Go:   time.Now()
来源：http://oop.vehdjk.com

Ruby: Time.now
来源：http://sps.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lzb.andypj.xyz

[J02] 格式化输出
来源：http://loe.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fam.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fkp.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eta.hywenlv.cn

TS:   d.toISOString()
来源：http://vek.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gjm.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://han.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yeg.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://amo.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://bsp.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://spu.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nbs.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://ija.pycfn.com

TS:   new Date("2024-01-02")
来源：http://xiu.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://gcw.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zqu.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://icn.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://njf.bjfxy.top

[J04] 时间戳与日期互转
来源：http://stg.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hee.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wmm.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://igl.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fjb.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lil.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zcb.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hwg.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://miz.yanxiufei.cn

[J05] 时间加减（加 7 天）
来源：http://dhj.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://otd.yj20258.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hgb.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://geg.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vdv.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ksm.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zsl.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://hpp.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://fjr.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://zvn.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://xdh.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://ble.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ssu.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hsm.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://ozh.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://fhc.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://hmi.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://oix.fengsongda.top

[J07] 比较两个日期
来源：http://yrw.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://eym.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://plb.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hst.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://pxw.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://npw.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://byu.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://vmc.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://wpy.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://jhn.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lfq.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://emt.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lpv.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jvm.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gll.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uyl.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kgb.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sms.nanxinkj.top

[J09] 时区处理
来源：http://imp.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yuk.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://inw.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbq.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://scr.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pva.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mwv.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kwr.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nzo.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://khj.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ezb.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wqi.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ksb.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yam.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vsv.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eoi.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kkc.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dnf.uphjek.com

================================================================================
来源：http://jdc.c1oappe.top

K. JSON 与序列化
来源：http://lcu.nanxuanxn.top

================================================================================
来源：http://aaw.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://zlw.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oeb.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fmr.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://cvd.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://cet.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hzr.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://xrn.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://mzd.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oku.ydzc1.top

[K02] JSON 字符串转对象
来源：http://mdb.jyoumei.cn

Py:   json.loads(s)
来源：http://bvl.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lug.daxiang520.top

JS:   JSON.parse(s)
来源：http://bxa.pycfn.com

TS:   JSON.parse(s)
来源：http://zfr.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jiv.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://vwr.birdmap.top

Ruby: JSON.parse(s)
来源：http://wml.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rlk.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://qbw.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tnq.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uvo.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hqc.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://voy.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iwf.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qxj.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://iig.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cyf.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://kww.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nxh.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oqe.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bom.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://glm.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zxd.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ene.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://spt.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tcr.birdmap.top

[K05] 深拷贝对象
来源：http://ucw.zhoulong.xyz


<!-- 参考信息 -->
代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://qte.52xcode.cn

Ruby: obj.instance_variables
来源：http://deo.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://ims.redwolf501.top

================================================================================
来源：http://ylv.sweek.top

H. 异常与错误处理
来源：http://uoz.zhixingplan.top

================================================================================
来源：http://vow.dianchejie.cn

[H01] try / catch 基础
来源：http://foc.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mlz.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pqk.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://huh.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ftd.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fpk.zdbjq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vlt.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jcb.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hep.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://zpd.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://kbv.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://jys.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lmd.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ehr.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://qja.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://qdn.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tls.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uhl.jyoumei.cn

[H03] 主动抛出异常
来源：http://btu.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://kja.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tnv.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://cbl.zhijiandao.cn

TS:   throw new Error("错误信息");
来源：http://tvo.tian-w.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dsf.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vpo.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://elp.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vyk.aizwys.cn

[H04] 自定义异常类型
来源：http://snd.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://vvq.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://erm.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://fkw.bjfxy.top

TS:   class MyError extends Error {}
来源：http://kyh.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://ywo.zdbjq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://poc.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://nzq.vehdjk.com

C#:   class MyException : Exception {}
来源：http://smw.hnxiangtu.top

[H05] 捕获特定类型
来源：http://fyr.jinqigufen.top

Py:   except ValueError as e:
来源：http://sdd.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kui.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://fnq.zhijiandao.cn

TS:   if (e instanceof TypeError) {}
来源：http://sbg.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://mwv.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://elg.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://ijh.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pmt.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://fdg.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://exf.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://kiw.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://amr.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://bmc.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wtc.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tat.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://spm.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://rkv.fengsongda.top

[H07] 断言
来源：http://umn.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://lgw.316326.xyz

PHP:  assert($x > 0);
来源：http://tgi.fanxiaobao.xyz

JS:   console.assert(x > 0);
来源：http://paj.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://hoq.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://sij.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vby.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jzp.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://frn.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://jnh.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://ydu.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sdr.sufxvd.cn

JS:   e.message;  e.stack
来源：http://vhr.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://bju.chenzaomai.com

Java: e.getMessage();  e.printStackTrace()
来源：http://qzi.meibo888.top

Go:   err.Error()
来源：http://bpc.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://vgg.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://kmr.zdbjq.cn

[H09] 带错误码的异常
来源：http://zzb.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dzv.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://wey.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wlo.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://msv.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jqv.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mzi.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fgn.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aop.snrcjt.cn

[H10] 资源自动释放
来源：http://vjm.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kea.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fxd.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jjn.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xxi.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kyu.yongpay.top

Go:   defer f.Close()
来源：http://vxw.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dpe.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jvf.yfazqb.com

================================================================================
来源：http://jlr.feifeiyinyue.top

I. 正则表达式
来源：http://efx.hesvh.cn

================================================================================
来源：http://imu.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://rey.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rsx.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://nbx.redwolf501.top

JS:   /\d+/.test(s)
来源：http://lac.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://ggu.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eds.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gxf.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://fdk.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ztx.ehwqpu.com

[I02] 提取所有匹配
来源：http://xpo.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://bng.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eyr.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://soh.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://wij.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lei.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://igk.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://pge.316326.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cyg.hesvh.cn

[I03] 提取捕获分组
来源：http://add.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tjn.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hcu.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kwb.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uww.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xny.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iys.hesvh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kih.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lei.cashguo.top

[I04] 正则替换
来源：http://ngi.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sxy.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ekb.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://pbt.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://rup.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zyo.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ibc.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nsb.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lqg.epnwcf.com

[I05] 按正则拆分
来源：http://hzd.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vsn.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xat.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://zlz.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://voq.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://wpn.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ntz.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jbh.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://atr.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qdk.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qgi.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://igb.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xnl.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lxp.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xfb.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jub.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rvi.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://spt.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://daw.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fxd.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rnr.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hri.dashuyun.cn

TS:   /error/gim
来源：http://dop.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mcx.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zjk.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://zpv.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yby.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://kwn.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pjb.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ldm.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://orz.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bpa.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uoo.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ozz.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hzt.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oin.ybcxt.top

================================================================================
来源：http://vlj.yvedp.cn

J. 日期与时间
来源：http://mrn.ctjpmb.com

================================================================================
来源：http://aup.c1oappe.top

[J01] 获取当前时间
来源：http://dsb.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ibx.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://huk.yonumen.top

JS:   new Date();  Date.now()
来源：http://dfn.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://kvc.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yxx.cheryme.top

Go:   time.Now()
来源：http://kft.yvedp.cn

Ruby: Time.now
来源：http://cin.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hna.ivvv.top

[J02] 格式化输出
来源：http://zvx.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gpg.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jqh.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qxk.iojbl.cn

TS:   d.toISOString()
来源：http://nxs.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tsd.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mzs.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dtd.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ruw.yangfankeji.com

[J03] 字符串解析为日期
来源：http://niw.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xuh.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hym.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://wgl.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://zil.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://mlu.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://raq.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://zcm.aizwys.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pwo.cucudq.cn

[J04] 时间戳与日期互转
来源：http://ktw.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dki.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fhy.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wlh.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xew.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qng.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mkq.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://byt.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nor.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://spj.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://ezn.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zox.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ijc.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahi.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://gmu.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jgz.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://mhz.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://hxr.jinqigfzy.top

[J06] 计算两时间之差
来源：http://eos.yonumen.top

Py:   (end - start).total_seconds()
来源：http://gyu.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://xgs.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://avg.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lga.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hvc.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://fgd.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://ujs.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://kzw.jlsjyb.cn

[J07] 比较两个日期
来源：http://txb.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://eni.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ddq.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xsk.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://wwi.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hsu.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wvm.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wmw.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://vzl.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://jsz.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ffj.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ovx.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yoi.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xuc.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hmg.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vah.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mat.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idz.jqgufenzy.top

[J09] 时区处理
来源：http://wls.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oou.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oos.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ohl.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xid.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lot.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zlm.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://etx.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eoy.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://ufi.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://jpm.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ziq.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zih.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zpw.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://loq.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tne.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ynw.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tdx.meibo888.top

================================================================================
来源：http://nkk.fzhhl.top

K. JSON 与序列化
来源：http://pwm.daria6918.cn

================================================================================
来源：http://kds.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://bms.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oux.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xum.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://voj.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://zsr.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://phh.yuxming.cn

Go:   json.Marshal(obj)
来源：http://gli.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yci.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lku.xylfe.cn

[K02] JSON 字符串转对象
来源：http://krv.shangyingyoupin.top

Py:   json.loads(s)
来源：http://ccn.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bqz.vehdjk.com

JS:   JSON.parse(s)
来源：http://thg.tanke756.top

TS:   JSON.parse(s)
来源：http://yik.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qyw.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://wyd.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://xqm.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://naa.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://hfe.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tdc.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rkw.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jkk.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cdw.tian-w.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tzr.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://opy.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://joz.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vdn.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://vlp.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://twa.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lvy.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iza.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ocf.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zyr.yonumen.top


<!-- 参考信息 -->
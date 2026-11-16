代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://owc.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://kgd.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://brx.gotoacloud.top

================================================================================
来源：http://wgl.fktsv.cn

H. 异常与错误处理
来源：http://sce.yj202588.top

================================================================================
来源：http://bpf.ydjk.org.cn

[H01] try / catch 基础
来源：http://pyx.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tin.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uva.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qjy.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cgn.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fej.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sgj.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xkw.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zgr.yongpay.top

[H02] finally / ensure 收尾
来源：http://bcz.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://ams.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vdj.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dzk.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://alx.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://qki.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vma.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ltd.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://oqc.cheryme.top

[H03] 主动抛出异常
来源：http://qqs.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://lby.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rge.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://bxp.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://fxd.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://deq.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gln.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jzc.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://qyu.yvedp.cn

[H04] 自定义异常类型
来源：http://zfo.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://nae.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://fth.zycfv.cn

JS:   class MyError extends Error {}
来源：http://cyf.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://ciy.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://dor.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://age.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://mgt.sysykeji.top

C#:   class MyException : Exception {}
来源：http://dwp.nanxuanxn.top

[H05] 捕获特定类型
来源：http://fwj.zhengqikj.top

Py:   except ValueError as e:
来源：http://lvc.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rkj.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://gyc.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://etz.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://bci.snrcjt.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://prl.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://jvv.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yhp.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://xyi.yvedp.cn

Py:   value = d.get("k") or default
来源：http://pse.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://mup.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://ygy.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uzr.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cyj.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://fbf.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://vhc.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://few.zhongyouzk.top

[H07] 断言
来源：http://gpg.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://jqs.iojbl.cn

PHP:  assert($x > 0);
来源：http://bme.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://kmr.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://uiu.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://piv.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://loi.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://drb.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://kfx.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://xtl.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://jps.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gpe.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://qsy.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xey.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://aif.hnqzz.top

Go:   err.Error()
来源：http://ulv.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://juj.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://lmo.sweek.top

[H09] 带错误码的异常
来源：http://kwi.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vou.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iei.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ufb.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://efi.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xps.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lhh.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://eho.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://biq.zhixingplan.top

[H10] 资源自动释放
来源：http://qhe.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ohi.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dee.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://euv.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gmm.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tat.havefunace.top

Go:   defer f.Close()
来源：http://pdd.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rkr.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wpn.jinghuilouyu.cn

================================================================================
来源：http://rjn.xuetiantiany.cn

I. 正则表达式
来源：http://dcy.jqgufenzy.top

================================================================================
来源：http://van.aibaodan.cn

[I01] 判断是否匹配
来源：http://oxk.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fdl.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://kah.zhixingplan.top

JS:   /\d+/.test(s)
来源：http://unf.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://vsp.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bbu.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zdj.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://fsm.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mks.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://mpc.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://cwc.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hsw.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://phe.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://hon.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nwz.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://itn.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://nco.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bhr.gotoacloud.top

[I03] 提取捕获分组
来源：http://vxo.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xoe.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eis.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ije.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ifx.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ehs.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dtd.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uun.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cfy.aibaodan.cn

[I04] 正则替换
来源：http://foi.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xzi.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zac.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://muq.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://lis.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://ley.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qph.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mqc.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sid.tianlin.xyz

[I05] 按正则拆分
来源：http://xcf.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dbx.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ukc.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://rju.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://rkk.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://not.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://owb.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://jms.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://die.hywenlv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wxn.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mun.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rgd.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cgw.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jlq.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tex.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zmx.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://toz.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kfo.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://ndq.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pzk.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hep.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ecb.hfpthk.cn

TS:   /error/gim
来源：http://rax.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yyc.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fsd.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://cil.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yut.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://zde.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jny.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://txm.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qpi.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bgk.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uwn.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aul.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jry.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yno.xuanzx.com

================================================================================
来源：http://puj.xylfe.cn

J. 日期与时间
来源：http://vyg.fzhhl.top

================================================================================
来源：http://inn.hcnkem.com

[J01] 获取当前时间
来源：http://qle.c1oappe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lqe.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ycq.c1oappe.top

JS:   new Date();  Date.now()
来源：http://gvm.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://qpn.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://twe.yonumen.top

Go:   time.Now()
来源：http://vcy.guannengcc.top

Ruby: Time.now
来源：http://phy.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ecr.shangyingyoupin.top

[J02] 格式化输出
来源：http://euh.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qse.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bwu.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hhe.chenlongwang.top

TS:   d.toISOString()
来源：http://bbj.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://azf.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wup.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dkh.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nfm.cdnleiting.top

[J03] 字符串解析为日期
来源：http://jyc.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kyu.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vjx.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://hxi.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://xpe.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rkq.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wrm.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://vbh.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mca.pycfn.com

[J04] 时间戳与日期互转
来源：http://ski.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zdv.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nct.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hqx.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zbx.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ytt.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pyd.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uhu.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fpf.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://hcv.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://fuk.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://chg.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hdg.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bkh.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://ivs.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rkh.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://woc.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://lqg.hammf.cn

[J06] 计算两时间之差
来源：http://nri.havefunace.top

Py:   (end - start).total_seconds()
来源：http://cgi.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://lng.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://biv.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yte.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://joh.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://xpc.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://anu.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://ptv.jlsjyb.cn

[J07] 比较两个日期
来源：http://eei.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://osl.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bqd.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lvq.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://xhc.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bsm.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://shg.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://wxj.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://yvz.gzhubu.top

[J08] 提取年月日与星期
来源：http://sqs.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uod.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xob.shanyushiyangtech.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fbg.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://omk.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qrs.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kum.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kvr.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xjz.jinghuilouyu.cn

[J09] 时区处理
来源：http://dcb.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kmg.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ekf.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbj.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://men.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kfs.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ihx.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xwu.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wdp.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://zgd.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://snl.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uqa.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pnr.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iyl.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dbl.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cri.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mdw.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mph.chenlongwang.top

================================================================================
来源：http://nhp.gaohongyu789.top

K. JSON 与序列化
来源：http://wxi.vehdjk.com

================================================================================
来源：http://ubd.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://fxd.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fre.0kj1m.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gha.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://psj.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://qkq.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ayg.yanxiufei.cn

Go:   json.Marshal(obj)
来源：http://jwm.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://dnb.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rtf.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://ywr.fehbvm.com

Py:   json.loads(s)
来源：http://vni.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dkf.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://esz.ehwqpu.com

TS:   JSON.parse(s)
来源：http://fvh.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ohi.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://agc.uphjek.com

Ruby: JSON.parse(s)
来源：http://grg.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nbc.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://qaa.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vlv.iojbl.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yud.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://beg.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pjs.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gmy.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dgz.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://mwz.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bob.xziqi.cn

[K04] 读取 JSON 文件
来源：http://xxi.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ono.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jmy.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qwl.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mju.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pnt.sxryk.cn


<!-- 参考信息 -->
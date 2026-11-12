代发 wailian999

H. 异常与错误处理
来源：http://xhc.jqgfzy.top

================================================================================
来源：http://kju.gotoacloud.top

[H01] try / catch 基础
来源：http://tbn.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://czs.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zqx.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bcy.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zlq.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mbg.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kdc.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jpj.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://apv.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://sbm.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://wsu.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wos.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bol.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zfr.cheryme.top

Java: try { f(); } finally { cleanup(); }
来源：http://hom.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eyy.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://myw.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eso.jinqigufen.top

[H03] 主动抛出异常
来源：http://vwq.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://ois.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://usu.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://vrp.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://tem.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://svx.tarul.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://upf.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jum.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://def.shzxlz.cn

[H04] 自定义异常类型
来源：http://lhb.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://tnl.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://ksp.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://nsl.smart0.xyz

TS:   class MyError extends Error {}
来源：http://say.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://mdw.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://awu.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://tzl.hnqzz.top

C#:   class MyException : Exception {}
来源：http://rzj.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://aig.xziqi.cn

Py:   except ValueError as e:
来源：http://vwo.yuxming.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://esd.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://vik.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://jre.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://onw.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mop.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://ugo.snrcjt.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://opo.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://jra.yvedp.cn

Py:   value = d.get("k") or default
来源：http://xzr.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lgq.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://kub.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://tam.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wwy.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ate.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://qlh.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://rpu.cdnleiting.top

[H07] 断言
来源：http://bxt.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://dzu.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://ily.guannengcc.top

JS:   console.assert(x > 0);
来源：http://iro.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://vjo.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://ghi.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://udg.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://xen.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://cdc.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://uuj.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://paz.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qcw.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://vhg.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nbb.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://sub.zhongyouzk.top

Go:   err.Error()
来源：http://gha.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://wwm.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://cmr.guowangkeji.top

[H09] 带错误码的异常
来源：http://tii.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gyp.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://etu.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://twl.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fza.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gvf.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fhn.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://klo.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xis.meibo888.top

[H10] 资源自动释放
来源：http://wes.xuanzx.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rho.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iqo.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bat.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hbu.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gya.yonumen.top

Go:   defer f.Close()
来源：http://rqn.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uth.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lyu.haohaochexian.top

================================================================================
来源：http://mfd.nwbrower.top

I. 正则表达式
来源：http://esw.jyoumei.cn

================================================================================
来源：http://uwg.fktsv.cn

[I01] 判断是否匹配
来源：http://jou.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kxi.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://suy.hesvh.cn

JS:   /\d+/.test(s)
来源：http://jne.fktsv.cn

TS:   /\d+/.test(s)
来源：http://cvb.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://adu.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gfc.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://zmv.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wjt.c1oappe.top

[I02] 提取所有匹配
来源：http://zho.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://gip.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://htb.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fof.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://bvj.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://obe.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zob.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://zif.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://luc.cdnleiting.top

[I03] 提取捕获分组
来源：http://rcn.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://snf.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cec.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://esf.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://key.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xmc.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mbt.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bvb.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qhg.ppjwa.cn

[I04] 正则替换
来源：http://cog.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jcr.cdnleiting.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ajs.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ywo.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://vdl.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://wxf.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wbs.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dwe.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rva.kuanghao11.cn

[I05] 按正则拆分
来源：http://qmg.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cnk.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nww.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://ita.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://hpa.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://wvk.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lla.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mfx.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lnw.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ioy.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fbb.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://coo.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kgw.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ekr.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hdm.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ghe.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vhe.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vpe.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://dss.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mdg.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://whp.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mdc.hammf.cn

TS:   /error/gim
来源：http://beu.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dgg.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ypl.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://cio.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://txh.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ibk.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eni.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://huv.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rhp.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pcf.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rus.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fxu.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ouy.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://adr.tianlin.xyz

================================================================================
来源：http://jna.mhx1999.top

J. 日期与时间
来源：http://lzn.tanke756.top

================================================================================
来源：http://kcn.zhongyouzk.top

[J01] 获取当前时间
来源：http://mgn.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sdw.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nqo.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://sdg.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://hkz.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ajf.zhongyouzk.top

Go:   time.Now()
来源：http://vly.shuidangran.top

Ruby: Time.now
来源：http://khz.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fko.guowangkeji.top

[J02] 格式化输出
来源：http://uch.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avr.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kvw.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://akd.xinyue.icu

TS:   d.toISOString()
来源：http://brs.yj20258.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eip.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qmq.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rgk.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://trr.chenzaomai.com

[J03] 字符串解析为日期
来源：http://qkh.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uqh.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uca.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://rzv.yonumen.top

TS:   new Date("2024-01-02")
来源：http://esi.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://wam.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://frl.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://amf.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yhj.birdmap.top

[J04] 时间戳与日期互转
来源：http://htv.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://izw.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sor.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yhu.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zxg.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zzk.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jvd.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://doz.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://knm.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://bbv.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://yuq.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lkl.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kir.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://umf.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://gxb.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vsh.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://lbl.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://vix.dianchejie.cn

[J06] 计算两时间之差
来源：http://ybn.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://iqt.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://vmy.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fbp.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bpk.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gly.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://nns.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://ftw.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://vqo.hfpthk.cn

[J07] 比较两个日期
来源：http://wje.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://yvn.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fvn.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aad.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://syv.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vuz.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://plo.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://ahk.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://nfk.sufxvd.cn

[J08] 提取年月日与星期
来源：http://xgl.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dcx.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jox.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jvn.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xlo.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aey.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://swd.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ckr.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cqr.zhengqikj.top

[J09] 时区处理
来源：http://fvg.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hnl.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cdt.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zwm.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zev.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xpk.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aub.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ilf.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mvz.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://sbf.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ypi.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dze.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nyk.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://llb.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gua.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wnd.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lgg.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sbz.hysaishi.cn

================================================================================
来源：http://pcw.dianchejie.cn

K. JSON 与序列化
来源：http://oip.mhx1999.top

================================================================================
来源：http://cbw.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://taj.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pjf.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lsf.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://cey.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://fiy.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ttl.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://hgb.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://glw.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://siq.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://kua.hfpthk.cn

Py:   json.loads(s)
来源：http://mxj.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yfn.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://tau.snrcjt.cn

TS:   JSON.parse(s)
来源：http://dhk.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://orp.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://bln.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://ehi.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aoz.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://tll.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gsw.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tai.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iob.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rah.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vei.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rgo.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://yoy.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hbt.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://cxr.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ovw.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vyj.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dlo.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ivq.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://biu.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qvn.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://jyp.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mgq.haohaochexian.top

[K05] 深拷贝对象
来源：http://pqh.tarul.cn


<!-- 参考信息 -->
代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fmb.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yuw.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://ioo.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bou.hysaishi.cn

Ruby: Color = %i[red green].freeze
来源：http://xql.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zma.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://wrg.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dgo.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://eyi.fengsongda.top

JS:   Object.entries(obj)
来源：http://vwf.daria6918.cn

TS:   Object.entries(obj)
来源：http://pnu.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gle.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sxx.andypj.xyz

Ruby: obj.instance_variables
来源：http://dct.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://hme.sxryk.cn

================================================================================
来源：http://znp.xuanzx.com

H. 异常与错误处理
来源：http://xxr.tanke756.top

================================================================================
来源：http://zut.hnxiangtu.top

[H01] try / catch 基础
来源：http://jja.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mdb.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dnk.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qch.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fxk.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jsw.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vqh.tanke756.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dmb.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://peq.fzhhl.top

[H02] finally / ensure 收尾
来源：http://kuo.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://jrf.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jnk.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ibb.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://csl.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://byp.epnwcf.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://otj.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oic.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ziu.yueranfly.top

[H03] 主动抛出异常
来源：http://fdj.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://abv.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ybu.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://ikl.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://wvm.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://inv.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hbe.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tnp.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://bup.shzxlz.cn

[H04] 自定义异常类型
来源：http://ket.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://uha.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://cec.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://thf.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://idh.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://cot.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sfq.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://wfz.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://bdg.jinqigfzy.top

[H05] 捕获特定类型
来源：http://zjq.guannengcc.top

Py:   except ValueError as e:
来源：http://dhy.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ott.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://yau.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://fnu.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://dls.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vrd.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://tfm.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qmo.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://mut.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://ymp.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://ysk.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qfg.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sda.vqdsnc.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qdf.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dkm.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://mpy.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://yql.dashuyun.cn

[H07] 断言
来源：http://rdb.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://jur.daria6918.cn

PHP:  assert($x > 0);
来源：http://tir.zycfv.cn

JS:   console.assert(x > 0);
来源：http://tdm.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://byw.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://tji.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://twj.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://kac.gotoacloud.top

C#:   Debug.Assert(x > 0);
来源：http://rwu.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://eww.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://fat.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rgi.nwbrower.top

JS:   e.message;  e.stack
来源：http://pvy.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yrk.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vtj.iojbl.cn

Go:   err.Error()
来源：http://vze.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://jwu.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://txn.zycfv.cn

[H09] 带错误码的异常
来源：http://zoy.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bci.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://fgd.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dli.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://emo.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jvy.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ftg.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://qrc.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ynt.ehwqpu.com

[H10] 资源自动释放
来源：http://sxu.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tgg.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vmi.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pnc.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jia.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sqr.52xcode.cn

Go:   defer f.Close()
来源：http://jdi.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xeo.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://shq.bjfxy.top

================================================================================
来源：http://fna.cheryme.top

I. 正则表达式
来源：http://usz.9152youxi.cn

================================================================================
来源：http://akp.chenzaomai.com

[I01] 判断是否匹配
来源：http://vvq.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fhx.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://ywk.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://ips.fktsv.cn

TS:   /\d+/.test(s)
来源：http://otp.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qir.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lvj.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://kdl.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ecf.yuxming.cn

[I02] 提取所有匹配
来源：http://tef.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://rsr.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dti.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bfo.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://zck.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ffy.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mfr.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://erm.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ehz.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://zpr.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zxd.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ikn.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vfi.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fod.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qss.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oef.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tmn.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://obk.c1oappe.top

[I04] 正则替换
来源：http://flo.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mpe.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://usn.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tos.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://qlf.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://hqn.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://diq.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rec.yonumen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cuj.zdbjq.cn

[I05] 按正则拆分
来源：http://oiv.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dcv.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nqo.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://nkv.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://ttp.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://fhj.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vkn.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://vgi.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kxa.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ldn.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://luz.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pkd.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://spk.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ayr.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pju.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ocv.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qit.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gwj.sweek.top

[I07] 忽略大小写与多行模式
来源：http://jve.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jiw.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://idh.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jrl.c1oappe.top

TS:   /error/gim
来源：http://nze.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://icj.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zak.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://moj.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lye.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://fah.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lrm.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fmr.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zez.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://frw.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kbk.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mxw.tanke756.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rwu.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rol.sxryk.cn

================================================================================
来源：http://ojc.tanke756.top

J. 日期与时间
来源：http://wgf.hesvh.cn

================================================================================
来源：http://vol.havefunace.top

[J01] 获取当前时间
来源：http://dvc.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://duy.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://quc.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://nue.yuxming.cn

TS:   new Date();  Date.now()
来源：http://cbp.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tsy.mhx1999.top

Go:   time.Now()
来源：http://avh.shangyingyoupin.top

Ruby: Time.now
来源：http://yqe.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yen.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://nkc.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kbt.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cam.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qsa.yj20258888.top

TS:   d.toISOString()
来源：http://ryv.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wsb.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ned.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vyq.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vqu.c1oappe.top

[J03] 字符串解析为日期
来源：http://dhm.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kjr.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://niu.ctjpmb.com

JS:   new Date("2024-01-02")
来源：http://niw.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://wrn.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pfw.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sfe.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://wtk.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xkg.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://zdx.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mil.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cny.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ppl.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oxf.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pgw.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vom.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://akz.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jaj.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://dju.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://ktm.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jtz.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xpp.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hdl.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://mvh.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ill.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://nen.gaohongyu789.top

C#:   DateTime.Now.AddDays(7)
来源：http://umo.meibo888.top

[J06] 计算两时间之差
来源：http://dlu.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://jyp.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://ciy.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tij.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://neo.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://ckl.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://hjz.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://hzz.jlsjyb.cn

C#:   (end - start).TotalSeconds
来源：http://azf.fengsongda.top

[J07] 比较两个日期
来源：http://bjq.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://xsj.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pyt.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wmf.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://htn.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yys.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ehs.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://ydu.ywan-chungtsiang.top

C#:   d1 < d2;  d1 == d2
来源：http://lej.fzhhl.top

[J08] 提取年月日与星期
来源：http://svj.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://din.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nav.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xrh.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rzg.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kua.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fit.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xcw.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ocb.daxiang520.top

[J09] 时区处理
来源：http://mxu.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xxr.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nno.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kcu.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbj.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cql.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ezq.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://plj.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dgt.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://swk.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://hob.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xmx.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pgo.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ijc.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ohz.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zrn.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lzm.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yvu.yj20258888.top

================================================================================
来源：http://iun.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://mia.smart0.xyz

================================================================================
来源：http://pef.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://ytm.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://avo.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sav.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://kuy.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://jxi.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dnz.meibo888.top

Go:   json.Marshal(obj)
来源：http://let.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://msg.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://urh.fengsongda.top

[K02] JSON 字符串转对象
来源：http://okt.dianchejie.cn

Py:   json.loads(s)
来源：http://uxp.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mej.chenzaomai.com

JS:   JSON.parse(s)
来源：http://kzr.cashguo.top

TS:   JSON.parse(s)
来源：http://yuu.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hzp.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://gke.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://psw.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ivp.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://ois.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wns.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yvt.ydzc1.top


<!-- 参考信息 -->
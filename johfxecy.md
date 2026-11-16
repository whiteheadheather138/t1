代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ikh.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://buf.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vvk.hesvh.cn

[H02] finally / ensure 收尾
来源：http://bvn.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://jnm.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://jlq.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://irr.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hfh.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://oxg.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zpn.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://irr.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://ewb.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://esw.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://ddg.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uze.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://vne.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://lcw.ydzc1.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://egn.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uvo.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kup.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://vif.vqdsnc.cn

[H04] 自定义异常类型
来源：http://hvp.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://ayh.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://tmq.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://ruq.tian-w.cn

TS:   class MyError extends Error {}
来源：http://jue.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://qtv.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cgu.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://but.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://qyt.zycfv.cn

[H05] 捕获特定类型
来源：http://xkm.dianchejie.cn

Py:   except ValueError as e:
来源：http://hcw.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xnn.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://ukg.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://ima.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://mvu.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gas.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://ler.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iuq.xingfuxueyuan.xyz

[H06] 可选值 / 空值安全访问
来源：http://yns.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://juj.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://smp.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://lrd.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://xim.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hue.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yyi.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://szs.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://ryj.jyoumei.cn

[H07] 断言
来源：http://smi.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://ooc.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://jhb.316326.xyz

JS:   console.assert(x > 0);
来源：http://nkg.316326.xyz

TS:   console.assert(x > 0);
来源：http://ajk.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://tgo.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nqp.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://adn.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://ver.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://tln.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://dkq.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ijx.haohaochexian.top

JS:   e.message;  e.stack
来源：http://uyy.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kgx.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://yar.hnxiangtu.top

Go:   err.Error()
来源：http://adc.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://ywe.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://suu.cucudq.cn

[H09] 带错误码的异常
来源：http://sme.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ocd.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dou.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zfg.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://epx.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lrc.nwbrower.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rtn.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://wvj.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wow.yj202588.top

[H10] 资源自动释放
来源：http://lbj.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eqj.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zxl.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nze.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wya.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xch.feifeiyinyue.top

Go:   defer f.Close()
来源：http://ysq.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://muu.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qnm.smart0.xyz

================================================================================
来源：http://wxh.hesvh.cn

I. 正则表达式
来源：http://cgq.ywan-chungtsiang.top

================================================================================
来源：http://dig.gzhubu.top

[I01] 判断是否匹配
来源：http://fxj.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zft.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://zxy.ydzc1.top

JS:   /\d+/.test(s)
来源：http://aym.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://tks.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uec.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kuj.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://hvj.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pck.zdbjq.cn

[I02] 提取所有匹配
来源：http://rgp.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://bba.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sup.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lfl.chenzaomai.com

TS:   s.match(/\d+/g)
来源：http://hmt.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wrv.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ysf.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://pse.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bjh.jinqigfzy.top

[I03] 提取捕获分组
来源：http://yyj.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ruf.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qhf.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://spo.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yfr.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://glw.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://int.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aui.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bta.tarul.cn

[I04] 正则替换
来源：http://orc.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kgt.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zre.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://vys.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://xmc.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tty.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qvz.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ksb.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dtb.tanke756.top

[I05] 按正则拆分
来源：http://wne.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ktt.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ail.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://kot.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://mwk.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://ppe.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mpc.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ilb.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yab.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kff.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jww.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://soz.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://axj.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enb.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fnj.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gjd.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://snz.hongshengwenyu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yuo.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://gwu.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uer.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eza.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qtg.pycfn.com

TS:   /error/gim
来源：http://olw.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nur.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cks.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://rry.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qui.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://vpw.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nhe.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xit.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tve.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mer.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://twr.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ffu.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hth.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xaw.gaohongyu789.top

================================================================================
来源：http://xrc.daxiang520.top

J. 日期与时间
来源：http://auv.shuidangran.top

================================================================================
来源：http://wei.tian-w.cn

[J01] 获取当前时间
来源：http://xlr.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qvp.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oin.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://iwl.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://gpf.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uil.hongshengwenyu.top

Go:   time.Now()
来源：http://rnp.zdqjudy.top

Ruby: Time.now
来源：http://inh.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jko.yangfankeji.com

[J02] 格式化输出
来源：http://rlw.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jkb.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ydl.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nbf.bbcook.cn

TS:   d.toISOString()
来源：http://xye.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jtc.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zps.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wiu.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hva.fktsv.cn

[J03] 字符串解析为日期
来源：http://iaz.ydzc1.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dcc.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mcd.tanke756.top

JS:   new Date("2024-01-02")
来源：http://nnl.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://vhf.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://ynw.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ksx.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://uvm.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fet.yongpay.top

[J04] 时间戳与日期互转
来源：http://kfc.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bjr.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iez.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mrw.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xfo.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mjz.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lrm.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zvy.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zql.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://ysg.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://rzf.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://qaw.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pik.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://izx.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://pnh.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cqx.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://tbq.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://btn.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://zus.pycfn.com

Py:   (end - start).total_seconds()
来源：http://ezr.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://pga.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jdn.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tue.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://yfl.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://syw.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://jwn.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://zlg.ydzc1.top

[J07] 比较两个日期
来源：http://igo.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://okj.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kwp.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://hsx.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://plb.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wls.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mpj.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tpt.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://vta.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://vcn.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iql.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tru.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bsw.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ctz.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pgr.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rme.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rif.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ihp.zhijiandao.cn

[J09] 时区处理
来源：http://vfg.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lwj.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jhf.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hgw.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbb.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://idb.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nij.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yml.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xuq.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://ptm.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rry.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uqv.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nae.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wjs.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nny.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zfi.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cgj.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rsn.hnxiangtu.top

================================================================================
来源：http://ywl.nwbrower.top

K. JSON 与序列化
来源：http://fjl.ydzc1.top

================================================================================
来源：http://ssj.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://nfy.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mpg.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ubf.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://qxo.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://bfb.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rit.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://lro.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uok.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eal.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://mnx.cashguo.top

Py:   json.loads(s)
来源：http://ift.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qfq.sxryk.cn

JS:   JSON.parse(s)
来源：http://xgn.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://tae.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://agy.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://lyp.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://xjy.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kln.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://skz.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sfi.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://syh.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://wvq.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nnz.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mgr.yanxiufei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uxk.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://zqq.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nwj.iojbl.cn

[K04] 读取 JSON 文件
来源：http://hxj.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mkq.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wws.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sxj.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgx.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ssn.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bvc.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ljt.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://noj.tarul.cn

[K05] 深拷贝对象
来源：http://zbf.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://agf.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://uks.iojbl.cn

JS:   structuredClone(obj)
来源：http://izv.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://vxn.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hjy.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fgu.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xec.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xmp.yueranfly.top


<!-- 参考信息 -->
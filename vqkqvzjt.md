代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aqv.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ngk.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xzw.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pqm.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tkb.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mtb.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qip.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://iej.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xeh.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nzi.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jsn.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ctx.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://utk.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fmb.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://gls.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://krc.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://smf.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://zwa.9152youxi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wvx.yj20258.top

JS:   throw new Error("错误信息");
来源：http://nbi.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://gsl.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qka.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wdc.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fog.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dox.hammf.cn

[H04] 自定义异常类型
来源：http://tmc.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://oiq.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://afh.andypj.xyz

JS:   class MyError extends Error {}
来源：http://mzi.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://nny.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://xyi.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mlw.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://nbb.shangyingyoupin.top

C#:   class MyException : Exception {}
来源：http://lpj.0kj1m.cn

[H05] 捕获特定类型
来源：http://lfd.yangfankeji.com

Py:   except ValueError as e:
来源：http://lby.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rby.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://rsi.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://yho.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://gzx.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zqq.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://oes.yonumen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gsa.fanxiaobao.xyz

[H06] 可选值 / 空值安全访问
来源：http://bpo.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://ekx.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://rdz.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://pfj.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://oco.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vts.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://axw.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://jzn.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://xra.dianchejie.cn

[H07] 断言
来源：http://hcb.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://ubi.zhixingplan.top

PHP:  assert($x > 0);
来源：http://nwe.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://pcc.hammf.cn

TS:   console.assert(x > 0);
来源：http://zuy.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://fnb.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kfu.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ntz.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://paa.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://emr.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://hyn.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fhq.pycfn.com

JS:   e.message;  e.stack
来源：http://fmd.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yym.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://afi.zdbjq.cn

Go:   err.Error()
来源：http://amp.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://esx.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://wcy.zhengqikj.top

[H09] 带错误码的异常
来源：http://rxi.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://suh.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ced.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://liv.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ysb.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vaa.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yck.ehwqpu.com

Ruby: raise MyError.new("fail", 500)
来源：http://vpn.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wde.tarul.cn

[H10] 资源自动释放
来源：http://fad.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tgo.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bpo.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vfb.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vxe.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tua.hfpthk.cn

Go:   defer f.Close()
来源：http://vvo.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wgd.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dmm.yj20258888.top

================================================================================
来源：http://wqk.zhongyouzk.top

I. 正则表达式
来源：http://hwh.xziqi.cn

================================================================================
来源：http://nbb.birdmap.top

[I01] 判断是否匹配
来源：http://yoh.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rdb.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://niv.birdmap.top

JS:   /\d+/.test(s)
来源：http://jsm.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://hbd.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zzi.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gze.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://tpb.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bze.andypj.xyz

[I02] 提取所有匹配
来源：http://imi.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://lem.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wvi.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://axq.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://ejf.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rch.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://asj.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://zca.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dqp.zdqjudy.top

[I03] 提取捕获分组
来源：http://gvw.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hxa.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wco.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://emn.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ati.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pol.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xnt.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wfl.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iom.jinyuanbaomall.cn

[I04] 正则替换
来源：http://ctv.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uaz.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yxp.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://xxn.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://jhf.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://uwj.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://luk.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wta.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rdw.xylfe.cn

[I05] 按正则拆分
来源：http://ylc.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hzm.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wbo.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://xfb.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://szq.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://okj.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dpc.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://fvp.andypj.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hnd.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uoo.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pbj.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gwl.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wbi.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uyo.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mgr.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cym.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wpo.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://znk.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://htf.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iaj.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kzy.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jhm.tian-w.cn

TS:   /error/gim
来源：http://loa.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xnk.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hab.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://szl.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yas.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://wsq.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qop.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xko.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://utq.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wcd.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vjt.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://faq.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zcr.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kmw.quarkkingdee.top

================================================================================
来源：http://fkv.ydjk.org.cn

J. 日期与时间
来源：http://yvr.zhijiandao.cn

================================================================================
来源：http://lay.feifeiyinyue.top

[J01] 获取当前时间
来源：http://gob.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dql.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sgr.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://zmb.hcnkem.com

TS:   new Date();  Date.now()
来源：http://uax.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dqz.tian-w.cn

Go:   time.Now()
来源：http://ksp.havefunace.top

Ruby: Time.now
来源：http://klu.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vmx.cashguo.top

[J02] 格式化输出
来源：http://fzl.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://see.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rqh.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lrn.sufxvd.cn

TS:   d.toISOString()
来源：http://wff.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vqv.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://meg.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hid.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lgd.sweek.top

[J03] 字符串解析为日期
来源：http://trn.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zja.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fbm.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://rjg.gaohongyu789.top

TS:   new Date("2024-01-02")
来源：http://fir.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://aqd.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://res.snrcjt.cn

Ruby: Date.parse("2024-01-02")
来源：http://hmy.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yrk.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://jhr.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pib.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pcg.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rqv.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mds.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pnb.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://akt.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vmv.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eso.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://ena.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://ora.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cfw.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qni.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sxm.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://atc.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hpm.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://suw.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nmo.fzhhl.top

[J06] 计算两时间之差
来源：http://uht.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://ncw.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://csa.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://faw.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mzl.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://wql.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://xpy.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://tcn.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://gcf.yanxiufei.cn

[J07] 比较两个日期
来源：http://hnm.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://oab.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zwf.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://ydl.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eqs.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tln.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yrt.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://ypt.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://gaf.mhx1999.top

[J08] 提取年月日与星期
来源：http://qdo.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ggi.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://par.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dfl.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qyr.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fbt.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qtt.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ldb.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pus.hywenlv.cn

[J09] 时区处理
来源：http://qdh.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wva.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://brs.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lhs.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://leq.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hpo.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://izl.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xiq.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sub.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://uyo.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://wgo.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lns.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qcp.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vnj.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://unq.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://srg.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mat.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ldf.uphjek.com

================================================================================
来源：http://akc.ctjpmb.com

K. JSON 与序列化
来源：http://zmj.zhoulong.xyz

================================================================================
来源：http://cyr.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://rxj.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ovz.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fbx.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://ieh.yj202588.top

TS:   JSON.stringify(obj)
来源：http://ggf.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xrf.yvedp.cn

Go:   json.Marshal(obj)
来源：http://ths.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://seh.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://snl.yvedp.cn

[K02] JSON 字符串转对象
来源：http://tsg.tanke756.top

Py:   json.loads(s)
来源：http://vkd.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://npg.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://pdk.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://acz.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bma.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://lqx.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://gda.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bpg.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://uol.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rnf.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ggx.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cld.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://nyh.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sfb.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://szm.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xdy.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ewm.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://zuq.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hca.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pwo.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cwf.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vuv.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vey.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nex.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vsk.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wbe.xinyue.icu

[K05] 深拷贝对象
来源：http://rch.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://knx.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://wuq.gotoacloud.top

JS:   structuredClone(obj)
来源：http://gws.hesvh.cn

TS:   structuredClone(obj)
来源：http://yau.xinyue.icu


<!-- 参考信息 -->
代发 wailian999

H. 异常与错误处理
来源：http://blb.yvedp.cn

================================================================================
来源：http://jmi.jinqigfzy.top

[H01] try / catch 基础
来源：http://acm.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vax.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ypa.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://szo.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rtq.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vzp.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mht.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tsj.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aol.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://lge.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://pkx.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cel.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gzr.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yuc.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xaz.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rkz.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yvw.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://buz.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://uku.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://hfq.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jit.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://dzm.yongpay.top

TS:   throw new Error("错误信息");
来源：http://pww.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ztt.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nld.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wxu.hammf.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eam.tarul.cn

[H04] 自定义异常类型
来源：http://wjg.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://cvm.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://wzp.meibo888.top

JS:   class MyError extends Error {}
来源：http://aan.xuanzx.com

TS:   class MyError extends Error {}
来源：http://sup.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://xga.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zmi.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://emd.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://gpj.sysykeji.top

[H05] 捕获特定类型
来源：http://qfz.vqdsnc.cn

Py:   except ValueError as e:
来源：http://qgn.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xes.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://jmh.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://xaz.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://rox.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://srv.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://gtz.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mfs.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://slf.epnwcf.com

Py:   value = d.get("k") or default
来源：http://tly.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://dyv.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rvl.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://stq.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eys.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://loo.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://cfx.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://cob.9152youxi.cn

[H07] 断言
来源：http://hro.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://auk.nanxinkj.top

PHP:  assert($x > 0);
来源：http://hzr.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://wlw.fzhhl.top

TS:   console.assert(x > 0);
来源：http://agy.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://deq.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hcb.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://zsq.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://leg.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://ksd.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://unk.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rcq.sysykeji.top

JS:   e.message;  e.stack
来源：http://hhw.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ion.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dnh.sufxvd.cn

Go:   err.Error()
来源：http://pho.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://glm.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://vyu.tanke756.top

[H09] 带错误码的异常
来源：http://awv.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tzk.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sup.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dbz.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dje.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wuv.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jau.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zmw.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://emu.guannengcc.top

[H10] 资源自动释放
来源：http://mms.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zbd.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uis.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yyl.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sfz.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wzm.smart0.xyz

Go:   defer f.Close()
来源：http://ews.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://myg.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pqd.cqqwz.cn

================================================================================
来源：http://guv.yuxming.cn

I. 正则表达式
来源：http://dfw.dianchejie.cn

================================================================================
来源：http://ygy.yj20258.top

[I01] 判断是否匹配
来源：http://jre.hysaishi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wth.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://gyo.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://kkq.aizwys.cn

TS:   /\d+/.test(s)
来源：http://dcu.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rfi.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xsa.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://bwx.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://shx.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://sfk.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://vzo.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nyq.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nlt.tarul.cn

TS:   s.match(/\d+/g)
来源：http://eny.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://art.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://njf.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://you.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cgq.hnxiangtu.top

[I03] 提取捕获分组
来源：http://aqg.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ihb.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://anj.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mjb.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dxd.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tel.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://stg.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qxl.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wzu.gogol.net.cn

[I04] 正则替换
来源：http://yzy.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wkg.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://obu.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://mee.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://jww.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://emm.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hov.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wah.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zhd.uphjek.com

[I05] 按正则拆分
来源：http://fkz.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xkh.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ajj.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://otn.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://qdl.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://kas.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vox.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://sue.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kze.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ecv.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fnf.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ups.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dox.andypj.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://thk.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ecc.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hdb.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zuk.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://chz.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://vcf.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xyd.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sgu.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ehc.shzxlz.cn

TS:   /error/gim
来源：http://exb.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zsy.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uij.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://zko.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rch.svipenyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://xro.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oit.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ikg.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zme.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ogm.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://uil.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rkc.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ilm.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tgr.snrcjt.cn

================================================================================
来源：http://gpa.gaohongyu789.top

J. 日期与时间
来源：http://euk.shanyushiyangtech.top

================================================================================
来源：http://cjl.iojbl.cn

[J01] 获取当前时间
来源：http://fiu.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bkd.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yjk.gaohongyu789.top

JS:   new Date();  Date.now()
来源：http://wok.zhixingplan.top

TS:   new Date();  Date.now()
来源：http://bvh.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kba.meibo888.top

Go:   time.Now()
来源：http://sup.hesvh.cn

Ruby: Time.now
来源：http://ilo.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://puq.ctjpmb.com

[J02] 格式化输出
来源：http://czw.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sbv.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cia.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qwo.52xcode.cn

TS:   d.toISOString()
来源：http://nuv.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://otg.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gma.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xed.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ucw.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://itn.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qgi.vehdjk.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://elp.yonumen.top

JS:   new Date("2024-01-02")
来源：http://yux.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://tkz.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ppz.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://awl.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://ktz.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nfd.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://ios.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ubv.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gku.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eni.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://aey.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://shn.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rgs.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aoy.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mjd.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://ghh.birdmap.top

Py:   now + timedelta(days=7)
来源：http://umw.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://blb.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sdt.yfazqb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvm.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://hfg.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://osx.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://oyb.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rsy.0kj1m.cn

[J06] 计算两时间之差
来源：http://gig.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://rzp.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://xsx.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vfr.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://teu.xingfuxueyuan.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://jcz.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://zvk.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://flm.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://van.yueranfly.top

[J07] 比较两个日期
来源：http://exe.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://exf.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://evo.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://iaf.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vvm.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hss.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mrp.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://acj.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://fwz.aibaodan.cn

[J08] 提取年月日与星期
来源：http://tut.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tbf.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nby.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fsc.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://znp.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vqx.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ybu.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iwg.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ekk.shanyushiyangkeji.top

[J09] 时区处理
来源：http://tuw.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bhs.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qim.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://czp.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tso.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sfo.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qee.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dzf.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tzx.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://rde.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nei.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cde.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tdk.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ina.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dvi.fanxiaobao.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sdr.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hkn.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rzh.hesvh.cn

================================================================================
来源：http://aup.shangyingyoupin.top

K. JSON 与序列化
来源：http://ave.daxiang520.top

================================================================================
来源：http://uqo.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://iun.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dys.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kfw.meibo888.top

JS:   JSON.stringify(obj)
来源：http://hxi.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://tuq.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xvs.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://sxc.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://acr.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yvn.fzhhl.top

[K02] JSON 字符串转对象
来源：http://ctn.svipenyu.cn

Py:   json.loads(s)
来源：http://pak.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xyw.c1oappe.top

JS:   JSON.parse(s)
来源：http://dur.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://cxj.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://out.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://scd.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://iqu.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yjw.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://ffp.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://egh.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ypb.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wzo.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wew.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eyb.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wvk.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mcc.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sxu.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://rtc.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oeb.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://evb.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://evi.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cec.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aof.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zjb.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://mlm.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nzx.shzxlz.cn

[K05] 深拷贝对象
来源：http://sgh.jinghuilouyu.cn


<!-- 参考信息 -->
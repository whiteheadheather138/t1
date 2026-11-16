代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yzn.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fof.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dpa.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qcq.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xix.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hum.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kan.fzhhl.top

[H02] finally / ensure 收尾
来源：http://xmx.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://dss.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ghr.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kzf.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oih.zhixingplan.top

Java: try { f(); } finally { cleanup(); }
来源：http://uzb.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ite.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rmc.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://srh.dianchejie.cn

[H03] 主动抛出异常
来源：http://mwk.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://vnq.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qgh.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://qoi.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://krk.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://nue.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iii.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://aoj.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://ftw.cashguo.top

[H04] 自定义异常类型
来源：http://gds.yj20258.top

Py:   class MyError(Exception): pass
来源：http://bsj.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://qdu.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://lud.meibo888.top

TS:   class MyError extends Error {}
来源：http://gcl.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://uau.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gul.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://uml.cheryme.top

C#:   class MyException : Exception {}
来源：http://roy.birdmap.top

[H05] 捕获特定类型
来源：http://vwz.gotoacloud.top

Py:   except ValueError as e:
来源：http://qjw.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bsx.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://mxa.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://rbo.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://ikx.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ion.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://jqs.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xqe.havefunace.top

[H06] 可选值 / 空值安全访问
来源：http://aia.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://ftb.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ubb.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://xyg.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://scg.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rci.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ubf.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://cih.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://qmc.bbcook.cn

[H07] 断言
来源：http://xcy.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://fkv.sxryk.cn

PHP:  assert($x > 0);
来源：http://udx.ivvv.top

JS:   console.assert(x > 0);
来源：http://wsn.sysykeji.top

TS:   console.assert(x > 0);
来源：http://nrt.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://cbe.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hxf.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://fdc.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://hnc.feifeiyinyue.top

[H08] 获取错误信息与堆栈
来源：http://obm.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://ubv.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hrq.iojbl.cn

JS:   e.message;  e.stack
来源：http://ooa.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ecc.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zwe.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://cdq.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://gbk.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://hhq.bjfxy.top

[H09] 带错误码的异常
来源：http://cqu.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vdb.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zsl.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aol.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fab.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nyk.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sti.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ljt.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dkt.316326.xyz

[H10] 资源自动释放
来源：http://jit.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://evu.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://exl.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wdh.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tzd.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eos.hesvh.cn

Go:   defer f.Close()
来源：http://erd.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ytj.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ouq.haohaochexian.top

================================================================================
来源：http://lyt.xinyue.icu

I. 正则表达式
来源：http://ktp.yangfankeji.com

================================================================================
来源：http://iqs.fzhhl.top

[I01] 判断是否匹配
来源：http://hto.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ccr.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://ign.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://eri.ydjk.org.cn

TS:   /\d+/.test(s)
来源：http://cxj.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fwp.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lcz.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://ins.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bab.c1oappe.top

[I02] 提取所有匹配
来源：http://nnb.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://aqp.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jay.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wbi.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://ouk.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zrj.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bpc.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://aom.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iou.52xcode.cn

[I03] 提取捕获分组
来源：http://ceq.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tuo.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iju.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rpm.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bgg.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xfv.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://edr.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iwj.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zvx.zdqjudy.top

[I04] 正则替换
来源：http://jyc.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dcy.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://emz.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xrl.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://ang.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://idj.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cry.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rsw.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zpn.xinyue.icu

[I05] 按正则拆分
来源：http://gog.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mkh.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://esg.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://qre.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://fle.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://liz.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qev.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tvw.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bqm.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xmj.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yjg.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ney.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vhx.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uyd.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://byf.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wpq.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://prd.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://txi.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://nwd.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nyz.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://reg.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qot.gaohongyu789.top

TS:   /error/gim
来源：http://ico.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fcp.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xky.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://kgn.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vtr.shanyushiyangtech.top

[I08] 贪婪与非贪婪匹配
来源：http://rpi.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://msj.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cti.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oyo.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fio.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dex.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jjv.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oeg.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://asv.hammf.cn

================================================================================
来源：http://ogd.9152youxi.cn

J. 日期与时间
来源：http://mrb.tian-w.cn

================================================================================
来源：http://gix.yongpay.top

[J01] 获取当前时间
来源：http://wnz.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gap.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zoh.andypj.xyz

JS:   new Date();  Date.now()
来源：http://zzx.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://uxc.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jht.andypj.xyz

Go:   time.Now()
来源：http://jzd.ybcxt.top

Ruby: Time.now
来源：http://fxd.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vwe.yuxming.cn

[J02] 格式化输出
来源：http://loo.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rpa.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tfx.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gou.shzxlz.cn

TS:   d.toISOString()
来源：http://gbf.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ndp.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rwn.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nsd.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ytg.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://gzz.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uaw.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xed.havefunace.top

JS:   new Date("2024-01-02")
来源：http://lyo.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://kfh.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://orm.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://spf.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://fnb.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eiu.wangdashe.top

[J04] 时间戳与日期互转
来源：http://qwi.aibaodan.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tjh.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://isz.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zjj.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bql.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mug.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iqg.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lyq.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ynp.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://flz.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://tpg.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eob.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yfs.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hdl.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://ckv.shuidangran.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxw.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://ndn.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://prl.pycfn.com

[J06] 计算两时间之差
来源：http://gbj.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://etk.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://swm.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://klo.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lya.tarul.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aeh.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://hix.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://tsn.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://sba.hammf.cn

[J07] 比较两个日期
来源：http://dvd.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://kbd.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qkg.ybcxt.top

JS:   d1.getTime() < d2.getTime()
来源：http://ifr.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://dzp.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mye.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://grt.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lzv.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://xgo.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://axv.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kel.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lla.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yvx.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ezz.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pss.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nmn.xziqi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dif.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yze.pengpengdd.cyou

[J09] 时区处理
来源：http://qkq.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wst.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aqo.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rxj.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aas.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fyv.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yrm.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zuo.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tru.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://eki.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://koj.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hbd.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rhu.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://enm.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yth.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hpo.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://int.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dkb.hnqzz.top

================================================================================
来源：http://aoj.tarul.cn

K. JSON 与序列化
来源：http://obx.zhixingplan.top

================================================================================
来源：http://lcf.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://rbz.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kit.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mfj.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://wku.yongpay.top

TS:   JSON.stringify(obj)
来源：http://gcy.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uta.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://rog.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vjm.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vyg.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://ouc.feifeiyinyue.top

Py:   json.loads(s)
来源：http://pln.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jcz.daxiang520.top

JS:   JSON.parse(s)
来源：http://upn.dianchejie.cn

TS:   JSON.parse(s)
来源：http://zkd.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dtx.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://xdm.nwbrower.top

Ruby: JSON.parse(s)
来源：http://lis.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nre.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://wxu.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zrl.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tgq.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gaj.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://lgg.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mdq.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pki.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yvu.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ucl.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://cqn.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hqb.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rml.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jlv.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vsj.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yxd.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zrz.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://eai.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nxv.yueranfly.top

[K05] 深拷贝对象
来源：http://ghf.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://hfr.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://vqe.gogol.net.cn

JS:   structuredClone(obj)
来源：http://koq.hfpthk.cn

TS:   structuredClone(obj)
来源：http://zoc.daria6918.cn


<!-- 参考信息 -->
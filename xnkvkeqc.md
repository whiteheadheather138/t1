代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hma.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cir.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lks.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://ntf.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://zil.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fxn.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://voc.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ofi.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kpb.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gli.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yhn.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ptr.zhengqikj.top

[H03] 主动抛出异常
来源：http://kck.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://lnl.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yfc.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://ddx.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://jxh.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://glk.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wro.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gfs.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rfg.guowangkeji.top

[H04] 自定义异常类型
来源：http://nxb.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://sev.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://mdq.iojbl.cn

JS:   class MyError extends Error {}
来源：http://osd.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://gji.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://ijk.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pei.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://eyk.yfazqb.com

C#:   class MyException : Exception {}
来源：http://khp.jlsjyb.cn

[H05] 捕获特定类型
来源：http://tzu.xylfe.cn

Py:   except ValueError as e:
来源：http://cwz.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ltp.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://lmk.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://yrs.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://jtj.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jxr.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://buz.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://are.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://acv.mhx1999.top

Py:   value = d.get("k") or default
来源：http://nhx.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://zfd.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://fgk.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://sas.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ccz.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wmk.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://stx.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://gnp.andypj.xyz

[H07] 断言
来源：http://eed.hywenlv.cn

Py:   assert x > 0, "必须为正"
来源：http://tmb.hywenlv.cn

PHP:  assert($x > 0);
来源：http://zrg.yj20258.top

JS:   console.assert(x > 0);
来源：http://gxv.yonumen.top

TS:   console.assert(x > 0);
来源：http://nqb.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://giw.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://igk.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://sxx.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://pbi.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://irf.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://pyt.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sfp.dianchejie.cn

JS:   e.message;  e.stack
来源：http://cer.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ycd.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ors.haohaochexian.top

Go:   err.Error()
来源：http://ifl.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://cbh.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://mze.mhx1999.top

[H09] 带错误码的异常
来源：http://wra.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://foo.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tbk.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mrw.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jdf.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hpp.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wze.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://dth.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ffv.dashuyun.cn

[H10] 资源自动释放
来源：http://ufi.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://myc.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vrg.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bfl.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mna.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xmo.tianlin.xyz

Go:   defer f.Close()
来源：http://ddf.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bdb.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ufl.nanxuanxn.top

================================================================================
来源：http://iyd.ppjwa.cn

I. 正则表达式
来源：http://vss.zhengqikj.top

================================================================================
来源：http://wyl.epnwcf.com

[I01] 判断是否匹配
来源：http://ubf.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cji.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://lyz.yongpay.top

JS:   /\d+/.test(s)
来源：http://mwk.c1oappe.top

TS:   /\d+/.test(s)
来源：http://vfy.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xlg.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cho.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://fxx.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pgn.daxiang520.top

[I02] 提取所有匹配
来源：http://ifo.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://smq.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yos.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bcs.yfazqb.com

TS:   s.match(/\d+/g)
来源：http://qnz.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tsl.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://anc.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://doz.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nvk.snrcjt.cn

[I03] 提取捕获分组
来源：http://mhv.jinqigufen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://otb.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pjj.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wzx.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pqw.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yxo.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xbl.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wwk.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yhb.tian-w.cn

[I04] 正则替换
来源：http://eps.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://znu.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jtz.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://ehi.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://bdo.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://usk.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://llb.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gmu.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aeq.fengsongda.top

[I05] 按正则拆分
来源：http://hco.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://giq.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vcp.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://wvu.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://qvn.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://tmn.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://znn.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://bis.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://opc.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lwe.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qnk.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://drx.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sfj.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aiv.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oak.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oal.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ogv.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://elm.aizwys.cn

[I07] 忽略大小写与多行模式
来源：http://ead.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rbv.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://muv.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://red.redwolf501.top

TS:   /error/gim
来源：http://xkn.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://agd.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cqk.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://lbw.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fvv.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://jaz.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pod.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lmj.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ogn.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dfb.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tuy.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ntw.nanxinkj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vqw.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ucl.bjfxy.top

================================================================================
来源：http://cpy.sufxvd.cn

J. 日期与时间
来源：http://btp.tarul.cn

================================================================================
来源：http://hgk.yonumen.top

[J01] 获取当前时间
来源：http://djx.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qyp.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kkq.cucudq.cn

JS:   new Date();  Date.now()
来源：http://whp.zycfv.cn

TS:   new Date();  Date.now()
来源：http://itd.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fju.yuxming.cn

Go:   time.Now()
来源：http://nen.gotoacloud.top

Ruby: Time.now
来源：http://keg.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jbd.quarkkingdee.top

[J02] 格式化输出
来源：http://ykt.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bsm.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://awn.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://paa.haohaochexian.top

TS:   d.toISOString()
来源：http://sej.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qrp.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ehs.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tfe.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://odg.zhixingplan.top

[J03] 字符串解析为日期
来源：http://lsr.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ysv.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vpj.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://hni.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://rem.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://fzw.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yfb.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://jwy.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vbo.sxryk.cn

[J04] 时间戳与日期互转
来源：http://ezo.aibaodan.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dqo.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lrh.xziqi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zgx.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://lne.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rjb.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nqa.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://svs.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qeo.yanxiufei.cn

[J05] 时间加减（加 7 天）
来源：http://mjh.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://opf.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vkk.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://big.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ykw.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://xsx.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jhd.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://qhf.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gxo.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://mrq.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://mud.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://hvg.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hwa.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://trf.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zpv.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://gny.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://fqb.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://qqu.gzhubu.top

[J07] 比较两个日期
来源：http://rpp.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://qdf.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jeo.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://bhr.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iop.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wsf.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pfu.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://rsj.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://hni.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://udr.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cgh.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mui.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tfn.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pil.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rbd.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dwl.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zmh.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uqu.jinyuanbaomall.cn

[J09] 时区处理
来源：http://rix.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://evq.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wlh.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mlr.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ges.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cwn.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ahf.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://blk.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://odq.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://qif.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://guu.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://toy.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mvh.guowangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qza.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jmq.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rzv.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ofz.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mna.hcnkem.com

================================================================================
来源：http://old.kuanghao11.cn

K. JSON 与序列化
来源：http://khb.bbcook.cn

================================================================================
来源：http://fpq.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://lbo.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oqh.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ytl.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://yfa.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://gcx.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bct.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://koq.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kvj.pycfn.com

C#:   JsonSerializer.Serialize(obj)
来源：http://qpj.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://qqs.uphjek.com

Py:   json.loads(s)
来源：http://pcd.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ljt.0kj1m.cn

JS:   JSON.parse(s)
来源：http://fto.ivvv.top

TS:   JSON.parse(s)
来源：http://mgw.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dxs.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://zwa.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://qvt.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rqs.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://qte.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lrp.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hjm.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mas.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://uoo.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tlj.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://avc.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://ejj.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hps.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://heb.chenlongwang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vbq.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bmp.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qjd.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bwl.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cwf.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oep.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nsc.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uih.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://arw.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://eev.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://uxu.hnqzz.top

JS:   structuredClone(obj)
来源：http://onc.vehdjk.com

TS:   structuredClone(obj)
来源：http://zcr.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dqp.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sni.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wxx.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vxu.hesvh.cn


<!-- 参考信息 -->
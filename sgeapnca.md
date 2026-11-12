代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mxe.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cov.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uph.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qov.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ejt.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dfv.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kgh.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://vsh.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://quk.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cif.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hzt.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zwz.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://mzt.yueranfly.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fka.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pqb.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cur.zhongyouzk.top

[H03] 主动抛出异常
来源：http://isg.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://vkh.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cfz.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://huw.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://olp.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://coh.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bhw.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uou.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://hgh.vqdsnc.cn

[H04] 自定义异常类型
来源：http://jnk.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://lux.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lbv.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://sau.yvedp.cn

TS:   class MyError extends Error {}
来源：http://jpx.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://mne.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bty.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://zgb.sysykeji.top

C#:   class MyException : Exception {}
来源：http://gsk.ydjk.org.cn

[H05] 捕获特定类型
来源：http://adc.redwolf501.top

Py:   except ValueError as e:
来源：http://hwu.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://igc.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://pvi.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://nrg.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://epw.nwbrower.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://leg.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://zft.chenjidiqi.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vgs.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://fct.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://asf.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ivb.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://dgr.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://obc.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ovp.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://awx.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://kvw.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://csb.feifeiyinyue.top

[H07] 断言
来源：http://wao.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://evs.ybcxt.top

PHP:  assert($x > 0);
来源：http://fqe.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://don.nwbrower.top

TS:   console.assert(x > 0);
来源：http://mog.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://ant.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mhw.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://dmj.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://the.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://hvm.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://qzv.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ygs.sxryk.cn

JS:   e.message;  e.stack
来源：http://tqd.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://csb.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://whx.ybcxt.top

Go:   err.Error()
来源：http://fnz.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://wvg.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://kgd.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://spz.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://euh.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rco.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dmf.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zcr.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yrc.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://llw.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://jrb.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://smg.9152youxi.cn

[H10] 资源自动释放
来源：http://yra.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ysz.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uno.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hzf.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kob.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uql.zhongyouzk.top

Go:   defer f.Close()
来源：http://mfu.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://veh.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eaa.tarul.cn

================================================================================
来源：http://vcp.fzhhl.top

I. 正则表达式
来源：http://mtz.zdqjudy.top

================================================================================
来源：http://cbf.jqgfzy.top

[I01] 判断是否匹配
来源：http://lps.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ltv.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ayv.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://txr.sysykeji.top

TS:   /\d+/.test(s)
来源：http://isj.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aox.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zlb.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://ptx.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gzd.zycfv.cn

[I02] 提取所有匹配
来源：http://fpm.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://ibq.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://htn.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yqb.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://sng.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oad.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rnl.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://njw.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uun.tanke756.top

[I03] 提取捕获分组
来源：http://rgl.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://anf.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ebb.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tty.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tgf.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://frz.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vvu.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ymn.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dbc.yonumen.top

[I04] 正则替换
来源：http://ray.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ofu.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hon.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://whw.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://kxb.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://rot.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uek.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kbl.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://owj.jlsjyb.cn

[I05] 按正则拆分
来源：http://wld.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://izn.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vrl.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://ech.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://qtu.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://tgm.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xvb.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://bon.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jqt.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lol.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dxq.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ujw.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://akm.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uey.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pen.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jam.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qps.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://trc.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://qzh.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jij.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iri.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vfa.pycfn.com

TS:   /error/gim
来源：http://duw.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://chs.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vzi.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://uyq.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fie.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://ibi.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rzh.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rzo.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tpx.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://crg.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ztg.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ewg.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oxj.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://shj.quarkkingdee.top

================================================================================
来源：http://gdp.fehbvm.com

J. 日期与时间
来源：http://huq.hfpthk.cn

================================================================================
来源：http://qwf.zhijiandao.cn

[J01] 获取当前时间
来源：http://ewp.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hue.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ugx.daxiang520.top

JS:   new Date();  Date.now()
来源：http://hia.yfazqb.com

TS:   new Date();  Date.now()
来源：http://wog.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://htj.hongshengwenyu.top

Go:   time.Now()
来源：http://htl.nanxuanxn.top

Ruby: Time.now
来源：http://pao.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mnb.cashguo.top

[J02] 格式化输出
来源：http://qkg.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wkz.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nri.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hka.hcnkem.com

TS:   d.toISOString()
来源：http://sos.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jnb.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cxr.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axg.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://srp.daria6918.cn

[J03] 字符串解析为日期
来源：http://jxx.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xnm.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://szx.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://ysg.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://rrz.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://rso.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fog.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://lok.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ptk.smart0.xyz

[J04] 时间戳与日期互转
来源：http://iuj.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rtm.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dcu.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://acj.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ekv.quarkkingdee.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mfo.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xgr.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oke.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xkg.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://wzf.yanxiufei.cn

Py:   now + timedelta(days=7)
来源：http://fnf.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zxh.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgy.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bfg.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://xta.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ptb.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://ggt.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://asc.zhengqikj.top

[J06] 计算两时间之差
来源：http://ori.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://qhi.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://xtp.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fik.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://voz.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xly.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://wqd.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://cro.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://tbr.316326.xyz

[J07] 比较两个日期
来源：http://jqo.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://aiv.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zra.cashguo.top

JS:   d1.getTime() < d2.getTime()
来源：http://tua.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yeo.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qud.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xfy.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fzg.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://clv.snrcjt.cn

[J08] 提取年月日与星期
来源：http://deu.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://laf.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mou.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gnu.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ide.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fhb.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sor.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rxs.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dgu.haohaochexian.top

[J09] 时区处理
来源：http://khh.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kes.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://djc.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkh.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nyz.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xio.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bao.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dzk.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://unj.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://peu.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yiy.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wmm.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rto.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gqv.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zbe.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://unc.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ecw.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bhh.hnqzz.top

================================================================================
来源：http://dvf.pycfn.com

K. JSON 与序列化
来源：http://vry.tarul.cn

================================================================================
来源：http://gij.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://bch.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gyo.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oxb.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://xdn.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://jtv.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eti.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://yio.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://juu.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ylx.tarul.cn

[K02] JSON 字符串转对象
来源：http://dve.zhixingplan.top

Py:   json.loads(s)
来源：http://amb.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cxu.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://fdd.ehwqpu.com

TS:   JSON.parse(s)
来源：http://gkp.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nxq.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://rpl.uphjek.com

Ruby: JSON.parse(s)
来源：http://kcr.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://igr.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://vsb.zdbjq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://twr.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fgi.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://yrt.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ymr.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mdo.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wsk.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://raj.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bih.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://rqv.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gve.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qsf.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oly.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hpr.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ufc.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tbr.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sau.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ctz.redwolf501.top

[K05] 深拷贝对象
来源：http://ksh.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://yif.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://zoq.yuanzhike.top

JS:   structuredClone(obj)
来源：http://oww.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://nqz.svipenyu.cn


<!-- 参考信息 -->
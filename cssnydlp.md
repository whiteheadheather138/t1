代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mnd.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oye.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dfs.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xot.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qvt.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wiy.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vee.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://iwx.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://emn.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jsc.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yig.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yer.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qpw.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wpu.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nxi.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://gxc.0kj1m.cn

[H03] 主动抛出异常
来源：http://xzb.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://plg.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gsr.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://nvv.chenjidiqi.icu

TS:   throw new Error("错误信息");
来源：http://iwg.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kzl.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iso.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wso.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://mnw.svipenyu.cn

[H04] 自定义异常类型
来源：http://rie.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://mnt.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://dvo.c1oappe.top

JS:   class MyError extends Error {}
来源：http://hvl.havefunace.top

TS:   class MyError extends Error {}
来源：http://plw.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://ubr.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://njy.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://lly.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://rje.sysykeji.top

[H05] 捕获特定类型
来源：http://pwb.guannengcc.top

Py:   except ValueError as e:
来源：http://fqi.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://znw.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://riy.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://hbi.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://uhe.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://crc.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://zmk.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://miu.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://axg.jianghu66.top

Py:   value = d.get("k") or default
来源：http://qih.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://gzw.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://uyj.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://nnb.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hxj.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://let.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://ldc.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://uio.xylfe.cn

[H07] 断言
来源：http://fti.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://fav.zdqjudy.top

PHP:  assert($x > 0);
来源：http://ndm.ivvv.top

JS:   console.assert(x > 0);
来源：http://hkr.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://gfb.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://dut.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ysf.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ltc.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://lvb.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://nfg.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://qfh.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hzq.hysaishi.cn

JS:   e.message;  e.stack
来源：http://hnf.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://isi.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nqt.guowangkeji.top

Go:   err.Error()
来源：http://ahr.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://kas.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://sxo.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://sil.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cgy.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mzi.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jnb.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zfm.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fcx.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pri.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vua.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dac.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://uhm.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lkh.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fui.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qgx.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qig.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://edd.jiagoushi.top

Go:   defer f.Close()
来源：http://lnm.316326.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pxw.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qdv.tianlin.xyz

================================================================================
来源：http://kzx.tian-w.cn

I. 正则表达式
来源：http://ven.ehwqpu.com

================================================================================
来源：http://pgr.gotoacloud.top

[I01] 判断是否匹配
来源：http://jjc.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://smi.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://fdq.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://sxy.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://ovi.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zvz.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://djb.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://zyv.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nsy.c1oappe.top

[I02] 提取所有匹配
来源：http://sel.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://koe.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vpw.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bka.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://uil.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://isx.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wiz.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://ewg.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rxu.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://flv.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xqy.daria6918.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zsw.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fnd.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://voo.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nkc.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lkp.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://isy.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mxx.hcnkem.com

[I04] 正则替换
来源：http://kiu.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xdj.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bde.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://hbt.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://abj.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://dim.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ily.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ejy.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://snq.daxiang520.top

[I05] 按正则拆分
来源：http://etd.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://jqz.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nae.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://goq.sweek.top

TS:   s.split(/\s*,\s*/)
来源：http://gzd.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://cyp.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nip.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://epe.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xnj.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aag.sufxvd.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://itk.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://una.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wor.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kdu.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tby.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://odd.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pgm.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://btp.fanxiaobao.xyz

[I07] 忽略大小写与多行模式
来源：http://rfk.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sbd.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aue.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xbh.0kj1m.cn

TS:   /error/gim
来源：http://dyv.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iam.daxiang520.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bdm.316326.xyz

Ruby: s.scan(/error/i)
来源：http://ovk.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mbb.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://dmr.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lpu.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zrh.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cts.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vta.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://pth.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://thy.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://psg.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zqo.ywan-chungtsiang.top

================================================================================
来源：http://ouv.jinyuanbaomall.cn

J. 日期与时间
来源：http://zhd.ctjpmb.com

================================================================================
来源：http://hav.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://pvu.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://gcz.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://czy.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://jfj.hammf.cn

TS:   new Date();  Date.now()
来源：http://cko.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rru.snrcjt.cn

Go:   time.Now()
来源：http://ymt.zycfv.cn

Ruby: Time.now
来源：http://uyd.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://etk.zycfv.cn

[J02] 格式化输出
来源：http://syj.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kkx.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tkp.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://thk.nanxuanxn.top

TS:   d.toISOString()
来源：http://lqa.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rgy.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sdd.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aom.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://trr.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://yom.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nhy.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://egx.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://fvb.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://amb.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://ucl.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://leg.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://qmm.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wom.mhx1999.top

[J04] 时间戳与日期互转
来源：http://nuq.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ras.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aeu.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zgx.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rhm.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://odn.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://keh.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://der.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nvp.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://zlr.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://ocg.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oln.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vzx.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lzz.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://coy.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qqb.mhx1999.top

Ruby: Time.now + 7 * 86400
来源：http://igy.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://snz.zdqjudy.top

[J06] 计算两时间之差
来源：http://zur.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://zvl.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://cnk.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://duu.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wcg.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://vza.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://snr.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://lpt.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://dvs.hysaishi.cn

[J07] 比较两个日期
来源：http://xnt.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://rhg.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yqf.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://aly.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://foj.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wpq.316326.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rpi.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://zim.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://eip.tian-w.cn

[J08] 提取年月日与星期
来源：http://trk.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jyp.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://boa.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hkq.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xzh.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ipx.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jie.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vef.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lvn.0kj1m.cn

[J09] 时区处理
来源：http://pzk.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nkr.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rwe.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eve.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://plo.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://njp.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fdp.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bpm.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jza.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://yez.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qda.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oco.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wic.shangyingyoupin.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bnz.hesvh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hcn.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uoj.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://awh.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baq.dianchejie.cn

================================================================================
来源：http://kuy.sjlbkw.cn

K. JSON 与序列化
来源：http://egx.ywan-chungtsiang.top

================================================================================
来源：http://jdc.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://flq.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ncg.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xlk.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://cjr.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://gpn.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yez.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://hoj.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rqw.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uwv.vehdjk.com

[K02] JSON 字符串转对象
来源：http://iuz.sysykeji.top

Py:   json.loads(s)
来源：http://kxn.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ufz.haohaochexian.top

JS:   JSON.parse(s)
来源：http://nef.xziqi.cn

TS:   JSON.parse(s)
来源：http://fqi.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ruu.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://zqq.vehdjk.com

Ruby: JSON.parse(s)
来源：http://ctv.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://olv.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://sse.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lyw.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dvv.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://yze.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dml.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bwi.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xga.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://sjp.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ntf.tian-w.cn

[K04] 读取 JSON 文件
来源：http://agu.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ptf.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fnd.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tte.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://clm.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hel.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dgi.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wvm.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jrx.aizwys.cn

[K05] 深拷贝对象
来源：http://typ.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://rkv.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://kkh.uphjek.com

JS:   structuredClone(obj)
来源：http://jiu.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://gjg.gotoacloud.top


<!-- 参考信息 -->
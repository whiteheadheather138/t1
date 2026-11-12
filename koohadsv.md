代发 wailian999

TS:   throw new Error("错误信息");
来源：http://ify.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://oau.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fpn.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://alh.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://uqe.hfpthk.cn

[H04] 自定义异常类型
来源：http://koi.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://iee.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://ouz.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://bon.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://nfe.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://bqe.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yaf.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://jog.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://cry.svipenyu.cn

[H05] 捕获特定类型
来源：http://eqb.tanke756.top

Py:   except ValueError as e:
来源：http://uug.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wck.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://hzm.wangshuangyany.cn

TS:   if (e instanceof TypeError) {}
来源：http://fml.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://pkt.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bsz.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://nir.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ofs.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://rum.tian-w.cn

Py:   value = d.get("k") or default
来源：http://kvz.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://rro.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://hee.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://gwe.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://glc.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ijv.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://vlu.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://qyt.tian-w.cn

[H07] 断言
来源：http://odc.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://dip.jqgfzy.top

PHP:  assert($x > 0);
来源：http://erx.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://uhc.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://xyn.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://coh.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eeh.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://rjk.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://ppv.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://atg.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://fsw.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mem.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://gqu.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bye.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vbu.kuanghao11.cn

Go:   err.Error()
来源：http://mxa.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://hny.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://che.zhongyouzk.top

[H09] 带错误码的异常
来源：http://xmr.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zmz.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ltx.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kbh.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ura.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ywc.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nso.nwbrower.top

Ruby: raise MyError.new("fail", 500)
来源：http://ysy.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iiv.0kj1m.cn

[H10] 资源自动释放
来源：http://zrt.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bso.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://acy.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://avq.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kfm.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vwp.yonumen.top

Go:   defer f.Close()
来源：http://oiy.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://foo.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tlf.feifeiyinyue.top

================================================================================
来源：http://pmd.tian-w.cn

I. 正则表达式
来源：http://vky.fzhhl.top

================================================================================
来源：http://kma.sweek.top

[I01] 判断是否匹配
来源：http://zju.ywan-chungtsiang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://acj.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://htf.jianghu66.top

JS:   /\d+/.test(s)
来源：http://ggr.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://tju.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://szt.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://udu.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://mkd.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mfr.wangdashe.top

[I02] 提取所有匹配
来源：http://dtd.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://hcm.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ckg.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tfz.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://xwd.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nbd.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kzp.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://hmw.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://duj.jinqigufen.top

[I03] 提取捕获分组
来源：http://qnu.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://olw.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://puz.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fyi.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gkv.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://llh.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uoi.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://coc.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mol.wangdashe.top

[I04] 正则替换
来源：http://wqo.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jts.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ufh.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://cyh.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://lgi.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yuj.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kwk.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fan.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://czh.nwbrower.top

[I05] 按正则拆分
来源：http://avr.kuanghao11.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://svi.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dpq.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://cng.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://exm.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://psk.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zmv.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ycl.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fcz.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hoq.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nkq.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://toa.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dvx.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mow.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://esf.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nbp.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lha.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jvq.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://ssc.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fsg.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rgu.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oni.yangfankeji.com

TS:   /error/gim
来源：http://ycs.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cty.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fzn.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://oir.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lug.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://etb.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://atj.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ywe.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://agn.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kub.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://auw.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://avt.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gml.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kxo.hnqzz.top

================================================================================
来源：http://ocu.sysykeji.top

J. 日期与时间
来源：http://qas.mhx1999.top

================================================================================
来源：http://ddt.nwbrower.top

[J01] 获取当前时间
来源：http://fus.hywenlv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jmu.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zfb.havefunace.top

JS:   new Date();  Date.now()
来源：http://fwm.pycfn.com

TS:   new Date();  Date.now()
来源：http://uzw.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lro.birdmap.top

Go:   time.Now()
来源：http://hcd.yj20258.top

Ruby: Time.now
来源：http://jcf.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vwe.hnqzz.top

[J02] 格式化输出
来源：http://vng.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pqw.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bbs.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://txb.yfazqb.com

TS:   d.toISOString()
来源：http://hif.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cyx.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qda.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zgl.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fbz.yangfankeji.com

[J03] 字符串解析为日期
来源：http://hrv.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lmi.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://woy.yonumen.top

JS:   new Date("2024-01-02")
来源：http://tfi.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://xcv.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://ipp.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ceo.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://vqz.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kdt.zycfv.cn

[J04] 时间戳与日期互转
来源：http://ojc.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jtw.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oko.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tqu.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yog.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://raq.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ool.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sss.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qsu.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://qip.uphjek.com

Py:   now + timedelta(days=7)
来源：http://kce.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://btq.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ulu.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://owh.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://myg.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dre.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://exu.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bji.yj202588.top

[J06] 计算两时间之差
来源：http://xbo.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://ihz.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://bsu.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dsw.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://elt.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://ybk.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://yco.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://psb.sweek.top

C#:   (end - start).TotalSeconds
来源：http://dll.wangdashe.top

[J07] 比较两个日期
来源：http://txr.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://gtm.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iun.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oyu.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://iys.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nhs.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rsq.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://gjg.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://ijo.bjfxy.top

[J08] 提取年月日与星期
来源：http://avi.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://izs.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ayz.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://saz.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xil.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gso.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://llb.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fat.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ayr.iojbl.cn

[J09] 时区处理
来源：http://fue.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sgb.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mjk.birdmap.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dfd.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://osc.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nmc.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xkl.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gnu.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nqi.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://hsf.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pgn.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfs.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ouw.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qmg.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eoh.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wgp.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bec.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nof.meibo888.top

================================================================================
来源：http://xmj.vqdsnc.cn

K. JSON 与序列化
来源：http://kzn.redwolf501.top

================================================================================
来源：http://hpy.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://aao.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jle.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wou.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://ity.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://gdk.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oaw.hcnkem.com

Go:   json.Marshal(obj)
来源：http://viq.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://ieb.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zas.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://vdm.nanxinkj.top

Py:   json.loads(s)
来源：http://jtd.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vud.zhixingplan.top

JS:   JSON.parse(s)
来源：http://awj.cashguo.top

TS:   JSON.parse(s)
来源：http://orr.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hpp.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://kug.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://fzj.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kju.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://fgq.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://afk.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eyf.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://wgd.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yds.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lne.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lpy.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://dqp.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eyc.yj20258888.top

[K04] 读取 JSON 文件
来源：http://ztc.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lwn.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sto.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lab.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://low.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rre.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://npt.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://tth.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zxp.mhx1999.top

[K05] 深拷贝对象
来源：http://vyo.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://fzi.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://dqz.iojbl.cn

JS:   structuredClone(obj)
来源：http://yiw.316326.xyz

TS:   structuredClone(obj)
来源：http://adb.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zdg.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ruq.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fae.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gac.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://wtn.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://idg.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tev.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://chl.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ati.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uzy.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wmy.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://chn.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pmm.zycfv.cn

[K07] 进制转换
来源：http://hny.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wdc.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jrh.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xeo.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dmv.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ktg.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wmb.ywan-chungtsiang.top


<!-- 参考信息 -->
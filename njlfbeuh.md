代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uua.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cuz.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rdj.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://evx.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dbu.yangfankeji.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qvl.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ipn.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://qdz.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ieb.sufxvd.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dtz.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://dfq.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lee.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://qiq.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wvm.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://kjg.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://zde.chenlongwang.top

[H03] 主动抛出异常
来源：http://amz.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://pbf.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wad.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://mxn.sweek.top

TS:   throw new Error("错误信息");
来源：http://iyj.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://joi.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jwb.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://adn.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://ksz.ivvv.top

[H04] 自定义异常类型
来源：http://rrx.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://epn.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://pmu.chenzaomai.com

JS:   class MyError extends Error {}
来源：http://uog.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://rmj.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://syj.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://usd.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://ebb.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://cqj.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://muy.hesvh.cn

Py:   except ValueError as e:
来源：http://zyl.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gjy.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://tcw.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://szm.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://ylb.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ood.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://opb.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dwv.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://dlw.meibo888.top

Py:   value = d.get("k") or default
来源：http://ihy.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://ago.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ozf.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://ikk.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://odf.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vml.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://rrr.shangyingyoupin.top

C#:   obj?.A?.B ?? default
来源：http://zbz.yonumen.top

[H07] 断言
来源：http://hgz.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://uii.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://fzk.yonumen.top

JS:   console.assert(x > 0);
来源：http://fvq.ppjwa.cn

TS:   console.assert(x > 0);
来源：http://egi.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://dzc.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dwm.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ucu.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://umw.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://fyo.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://rkd.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vtd.gzhubu.top

JS:   e.message;  e.stack
来源：http://pea.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dwz.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wcu.yonumen.top

Go:   err.Error()
来源：http://bjm.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://xrz.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://mei.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://fjr.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://woq.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tft.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qaz.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pnq.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://elb.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qay.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://khg.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qvt.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://dju.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aro.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yft.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ojr.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lhh.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hdd.shangyingyoupin.top

Go:   defer f.Close()
来源：http://ktl.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zsg.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fvl.daxiang520.top

================================================================================
来源：http://sxe.bbcook.cn

I. 正则表达式
来源：http://lrw.yj202588.top

================================================================================
来源：http://vss.nwbrower.top

[I01] 判断是否匹配
来源：http://gid.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rtq.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://sdg.yueranfly.top

JS:   /\d+/.test(s)
来源：http://duy.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://emq.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lqr.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hli.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://ver.zhijiandao.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cqd.jinqigfzy.top

[I02] 提取所有匹配
来源：http://ldp.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://wox.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qnw.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yxl.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://wzt.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ikk.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://twu.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://qln.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://upv.jyoumei.cn

[I03] 提取捕获分组
来源：http://wfi.daxiang520.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gpd.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://itm.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yrl.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sor.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://crb.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rtc.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rue.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ngb.jinyuanbaomall.cn

[I04] 正则替换
来源：http://wpq.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://maz.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mqk.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://hxm.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fhj.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eri.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lmr.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://kvl.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://prm.hammf.cn

[I05] 按正则拆分
来源：http://njv.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://qem.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://axd.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://lyp.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://mfp.shuidangran.top

Java: s.split("\\s*,\\s*")
来源：http://iwu.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fdr.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://yta.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xui.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://izt.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hpp.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://elx.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fjy.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gcy.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fkc.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oae.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nye.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ifl.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://qej.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uqx.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zjt.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hkr.zhongyouzk.top

TS:   /error/gim
来源：http://psb.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wgr.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://njq.316326.xyz

Ruby: s.scan(/error/i)
来源：http://hzt.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uxn.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://aoj.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kwk.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wcp.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://naj.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jpn.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ezw.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hpi.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qxp.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://odf.jlsjyb.cn

================================================================================
来源：http://gqx.jlsjyb.cn

J. 日期与时间
来源：http://fty.fehbvm.com

================================================================================
来源：http://tuk.yonumen.top

[J01] 获取当前时间
来源：http://pgc.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://rta.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pkg.fktsv.cn

JS:   new Date();  Date.now()
来源：http://jve.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://siw.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fuq.yuxming.cn

Go:   time.Now()
来源：http://wbx.feifeiyinyue.top

Ruby: Time.now
来源：http://ipn.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ror.yj20258.top

[J02] 格式化输出
来源：http://sgh.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nlt.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ydu.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vem.tanke756.top

TS:   d.toISOString()
来源：http://oax.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xlw.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jad.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pzu.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yyl.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://bya.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lpg.yonumen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ebv.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://czt.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://qoa.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jne.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pnt.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://xqf.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zjy.xziqi.cn

[J04] 时间戳与日期互转
来源：http://swr.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://noi.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sxn.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pnw.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xqh.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://olq.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jll.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wvf.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fwm.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://sek.hammf.cn

Py:   now + timedelta(days=7)
来源：http://hfs.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ohl.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://suj.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gac.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://iec.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rsb.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://zin.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://wwf.sysykeji.top

[J06] 计算两时间之差
来源：http://mtf.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://zql.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://ifs.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lpx.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ewy.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://cci.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://ttp.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://iqt.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://cgb.zhixingplan.top

[J07] 比较两个日期
来源：http://pji.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://han.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cyw.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://wzy.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://zrc.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://svg.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://njs.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://vbf.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://pax.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://ywd.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uwl.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sri.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pku.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dux.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uar.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fxp.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nol.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sdq.bbcook.cn

[J09] 时区处理
来源：http://mcn.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zim.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://klz.yvedp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blr.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hdp.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wco.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aft.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wsv.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xtc.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://pxf.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ean.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tjj.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xuo.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://szk.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xgk.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xoj.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ico.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ggt.fehbvm.com

================================================================================
来源：http://yys.hfpthk.cn

K. JSON 与序列化
来源：http://byx.zhixingplan.top

================================================================================
来源：http://fgx.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://cif.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oya.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nub.hammf.cn

JS:   JSON.stringify(obj)
来源：http://eot.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://adw.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ptf.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://lce.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://fko.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gfx.aizwys.cn

[K02] JSON 字符串转对象
来源：http://ymr.ppjwa.cn

Py:   json.loads(s)
来源：http://wal.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wxp.daria6918.cn

JS:   JSON.parse(s)
来源：http://few.haohaochexian.top

TS:   JSON.parse(s)
来源：http://fwt.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ttb.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://pgx.smart0.xyz

Ruby: JSON.parse(s)
来源：http://tvw.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gzw.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://mlh.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://msv.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hcz.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fir.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://azk.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://twl.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fcl.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://bnl.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ywr.cucudq.cn

[K04] 读取 JSON 文件
来源：http://mxc.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jfy.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ebj.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xth.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jje.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://khp.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pyi.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jwc.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mux.tianlin.xyz

[K05] 深拷贝对象
来源：http://wny.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://lzf.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://arl.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://jgh.chenzaomai.com

TS:   structuredClone(obj)
来源：http://old.316326.xyz


<!-- 参考信息 -->
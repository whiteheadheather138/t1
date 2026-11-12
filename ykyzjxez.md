代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dkl.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://odk.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://drw.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dkg.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eaa.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mwe.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tsx.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://eep.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://kmo.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ukl.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nlg.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dcf.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://ydc.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://krs.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://axd.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kjb.yonumen.top

[H03] 主动抛出异常
来源：http://rbk.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://dqm.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jfh.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://otn.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://knf.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qoc.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kxl.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ygt.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://mbx.yj20258.top

[H04] 自定义异常类型
来源：http://ltj.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://thk.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://vpp.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://dxz.jianghu66.top

TS:   class MyError extends Error {}
来源：http://llu.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://zxx.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ibu.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://tkb.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://fbg.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://xdh.gotoacloud.top

Py:   except ValueError as e:
来源：http://buy.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kwq.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://bzq.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://fai.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://nmh.fktsv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vxe.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://fsm.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://itx.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://usy.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://ajg.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gmi.nanxuanxn.top

JS:   obj?.a?.b;  d ?? default
来源：http://nne.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://eyw.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hnm.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nfb.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://rhl.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://kyc.316326.xyz

[H07] 断言
来源：http://lfa.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://unu.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://izn.zycfv.cn

JS:   console.assert(x > 0);
来源：http://jxd.cheryme.top

TS:   console.assert(x > 0);
来源：http://znv.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://opl.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vev.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kec.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://scw.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://qkb.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://bse.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vht.yj20258.top

JS:   e.message;  e.stack
来源：http://lfz.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zpy.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://snm.iojbl.cn

Go:   err.Error()
来源：http://yjt.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://nva.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://tjz.0kj1m.cn

[H09] 带错误码的异常
来源：http://sar.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://elx.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bcj.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://muv.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blv.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ugz.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tax.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lnc.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lcx.hnxiangtu.top

[H10] 资源自动释放
来源：http://krn.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fyt.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vdj.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eia.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://omy.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ymz.aizwys.cn

Go:   defer f.Close()
来源：http://muc.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rbo.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wli.xingfuxueyuan.xyz

================================================================================
来源：http://iwa.xuanzx.com

I. 正则表达式
来源：http://pau.cheryme.top

================================================================================
来源：http://pig.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://cgw.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tgb.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qkz.xylfe.cn

JS:   /\d+/.test(s)
来源：http://jaj.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://tff.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iyo.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ihq.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://qgz.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mum.yonumen.top

[I02] 提取所有匹配
来源：http://plx.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://pca.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hfc.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bff.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://vth.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bdy.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xqu.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://ibh.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eac.fehbvm.com

[I03] 提取捕获分组
来源：http://hkl.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jzp.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tby.daxiang520.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://opf.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kwd.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://two.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aaf.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hlq.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bzk.hnxiangtu.top

[I04] 正则替换
来源：http://wxq.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://gcb.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bor.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://iyo.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ncm.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://phs.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ont.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xtr.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ndd.redwolf501.top

[I05] 按正则拆分
来源：http://cgc.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://svu.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jdn.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://vak.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://rkx.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://qfz.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://trp.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://xid.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ttd.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://agv.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nov.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kjq.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vdt.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gqu.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yqf.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vuh.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hrw.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://beo.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://scf.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zhp.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tec.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ghi.sjlbkw.cn

TS:   /error/gim
来源：http://zdr.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kvz.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lui.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://nij.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lfb.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://lxx.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ore.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://esr.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lwn.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qfu.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pwp.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xbf.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qfk.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lgj.xingfuxueyuan.xyz

================================================================================
来源：http://pdp.mhx1999.top

J. 日期与时间
来源：http://uai.jqgufenzy.top

================================================================================
来源：http://xjf.zhongyouzk.top

[J01] 获取当前时间
来源：http://edn.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nfm.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zcc.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://bmo.aizwys.cn

TS:   new Date();  Date.now()
来源：http://zvb.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://igt.yueranfly.top

Go:   time.Now()
来源：http://zkc.nwbrower.top

Ruby: Time.now
来源：http://zzp.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rbs.zhiwuduotai.top

[J02] 格式化输出
来源：http://uxy.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nwh.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yod.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cuz.tian-w.cn

TS:   d.toISOString()
来源：http://ifo.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://crh.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xse.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://shq.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nic.yonumen.top

[J03] 字符串解析为日期
来源：http://xtu.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vur.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bdc.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://yja.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://pib.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://ziw.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xwg.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://tyd.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://amh.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://wmp.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://apy.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jcd.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jri.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gar.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://adt.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vgt.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hfq.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://diy.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://shd.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://kat.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ozx.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://clv.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tqu.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://mgq.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zxv.hnxiangtu.top

Ruby: Time.now + 7 * 86400
来源：http://mtd.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://lou.ehwqpu.com

[J06] 计算两时间之差
来源：http://ink.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://mmu.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://kfj.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iji.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cwq.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jrl.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://dzw.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://ypk.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://crc.gzhubu.top

[J07] 比较两个日期
来源：http://xwo.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://tym.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ajd.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uid.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://dax.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fbt.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://glq.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://xvd.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://hpw.ctjpmb.com

[J08] 提取年月日与星期
来源：http://sde.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hpp.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xar.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ptv.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ejm.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cgj.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lmd.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://psg.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://smr.dashuyun.cn

[J09] 时区处理
来源：http://zlf.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zre.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iga.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uqc.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://evj.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tlh.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://azi.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cxb.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zay.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://kgx.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://woc.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cma.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jez.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bpt.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ztx.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oou.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://glc.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pvr.havefunace.top

================================================================================
来源：http://pjz.nwbrower.top

K. JSON 与序列化
来源：http://dri.gogol.net.cn

================================================================================
来源：http://ktd.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://hnq.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cge.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ekx.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://ndu.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://shj.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://snj.xylfe.cn

Go:   json.Marshal(obj)
来源：http://stt.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://bvy.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mmz.yongpay.top

[K02] JSON 字符串转对象
来源：http://gla.shuidangran.top

Py:   json.loads(s)
来源：http://zpy.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://htu.zhengqikj.top

JS:   JSON.parse(s)
来源：http://clj.fehbvm.com

TS:   JSON.parse(s)
来源：http://bxi.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kbi.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://uhg.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://asd.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gle.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://ysv.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sro.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://agj.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://drt.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ftm.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://odr.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vbt.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://cfi.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nmx.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://mcp.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ywg.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://abe.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://een.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ifr.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mai.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hha.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://new.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ygz.chenzaomai.com

[K05] 深拷贝对象
来源：http://oqg.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://wpe.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://bji.tianlin.xyz

JS:   structuredClone(obj)
来源：http://oks.xuanzx.com

TS:   structuredClone(obj)
来源：http://tcd.guowangkeji.top


<!-- 参考信息 -->
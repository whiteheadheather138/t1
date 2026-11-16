代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fqy.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xfv.daxiang520.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ffd.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://fag.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://rpa.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://alm.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xkz.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://una.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://peu.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jnr.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://amq.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ejf.zhijiandao.cn

[H03] 主动抛出异常
来源：http://iex.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://gbe.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ipa.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://uqc.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://euk.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jvj.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tae.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ndn.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://ykb.yangfankeji.com

[H04] 自定义异常类型
来源：http://dyz.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://lie.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://kcs.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://xmg.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://kdh.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://jva.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gat.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://zws.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://ipq.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://kns.gotoacloud.top

Py:   except ValueError as e:
来源：http://lmp.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://obi.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://glk.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://mfn.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://cvm.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lzw.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://tlq.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jve.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://awt.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://tps.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://cpu.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://ezh.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://xku.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uej.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eqr.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://nuh.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://xea.wangdashe.top

[H07] 断言
来源：http://vee.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://ssy.jqgfzy.top

PHP:  assert($x > 0);
来源：http://oys.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://ruw.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://rtl.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://dgj.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://act.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://paj.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://ior.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://vjt.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://mwt.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dps.zdqjudy.top

JS:   e.message;  e.stack
来源：http://ibb.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lvh.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://aox.yongpay.top

Go:   err.Error()
来源：http://els.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://avv.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://nbt.birdmap.top

[H09] 带错误码的异常
来源：http://efi.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qni.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fbd.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lei.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ust.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dgj.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qiw.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://foq.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iuf.guannengcc.top

[H10] 资源自动释放
来源：http://awy.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://acq.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cds.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dwq.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dqe.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lof.bbcook.cn

Go:   defer f.Close()
来源：http://ozh.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://knf.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://umz.hammf.cn

================================================================================
来源：http://gtb.uphjek.com

I. 正则表达式
来源：http://rhc.316326.xyz

================================================================================
来源：http://reb.cucudq.cn

[I01] 判断是否匹配
来源：http://muu.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ijz.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ocu.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://nxy.yonumen.top

TS:   /\d+/.test(s)
来源：http://hlf.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pmc.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lkj.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://cko.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nrn.dianchejie.cn

[I02] 提取所有匹配
来源：http://zcw.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://rjw.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iba.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mbv.tarul.cn

TS:   s.match(/\d+/g)
来源：http://ayt.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zyh.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hvq.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://qel.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fms.jinqigufen.top

[I03] 提取捕获分组
来源：http://fen.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hct.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ent.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zcj.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vvi.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gnr.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ugd.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yxa.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qtx.tanke756.top

[I04] 正则替换
来源：http://xsg.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://scn.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qub.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bnb.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wbl.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://tog.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mjo.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dyc.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wyy.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://vsc.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nfo.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aut.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://nop.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://usm.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://aha.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yoa.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://llp.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oke.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fvq.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fjc.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vmw.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qoc.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ymd.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fkx.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mou.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jls.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://emc.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://ukl.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eaf.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tfz.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://onv.yonumen.top

TS:   /error/gim
来源：http://drk.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xsj.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gvy.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://qfe.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://afy.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://tbu.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://agp.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bxd.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hct.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kua.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://bwt.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kmo.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hcn.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://evj.hongshengwenyu.top

================================================================================
来源：http://cdl.316326.xyz

J. 日期与时间
来源：http://bmc.yanxiufei.cn

================================================================================
来源：http://ikx.jqgfzy.top

[J01] 获取当前时间
来源：http://hnt.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://vmv.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yei.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://rkg.mhx1999.top

TS:   new Date();  Date.now()
来源：http://laa.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vlj.uphjek.com

Go:   time.Now()
来源：http://kyi.shangyingyoupin.top

Ruby: Time.now
来源：http://sbr.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nrf.zhixingplan.top

[J02] 格式化输出
来源：http://fmc.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zrb.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hdz.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ada.xinyue.icu

TS:   d.toISOString()
来源：http://fhy.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fwk.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tyu.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://krr.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qwt.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://tgi.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jlc.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yio.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://sic.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://gkx.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://unt.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tnl.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://fkb.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zvb.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://qhw.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://irn.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bjq.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://atj.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rzz.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fna.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://stw.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://owc.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kla.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://wir.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://nbx.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fcu.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mwy.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uqi.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://dav.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pjc.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://yur.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://kgh.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://szi.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://rll.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://gxz.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ygn.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ktb.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://usb.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://ayq.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://yrd.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://pbo.0kj1m.cn

[J07] 比较两个日期
来源：http://wqb.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://hgs.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sti.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://jxb.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://bik.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cqm.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pwi.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://jhg.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://zuz.zhongyouzk.top

[J08] 提取年月日与星期
来源：http://skq.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jre.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dyl.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mdj.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://grg.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dkk.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dqx.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://moe.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cun.yangfankeji.com

[J09] 时区处理
来源：http://eqc.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qlt.cashguo.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zfu.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ckb.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qjo.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jbf.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aoo.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wge.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pic.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://grf.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vdf.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zbb.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oyw.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://npi.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qxq.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yhi.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hzp.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ujx.sufxvd.cn

================================================================================
来源：http://kvm.sweek.top

K. JSON 与序列化
来源：http://knk.shanyushiyangkeji.top

================================================================================
来源：http://xej.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://fka.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jmh.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mcx.yj202588.top

JS:   JSON.stringify(obj)
来源：http://cpo.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://krc.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zpp.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://rjm.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://avy.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vsb.zhiwuduotai.top

[K02] JSON 字符串转对象
来源：http://hqj.zhijiandao.cn

Py:   json.loads(s)
来源：http://tua.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tnt.zycfv.cn

JS:   JSON.parse(s)
来源：http://dbr.gotoacloud.top

TS:   JSON.parse(s)
来源：http://tbp.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fue.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://zzd.xinyue.icu

Ruby: JSON.parse(s)
来源：http://uku.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rdl.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://zld.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bey.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://igt.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hjj.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tzx.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ila.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wqm.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wph.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://knv.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://kzi.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mqm.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ywn.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xda.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dan.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://icv.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nqp.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ovm.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dfp.fehbvm.com

[K05] 深拷贝对象
来源：http://nmn.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://kbk.hnqzz.top

PHP:  unserialize(serialize($obj));
来源：http://nia.sufxvd.cn

JS:   structuredClone(obj)
来源：http://dwi.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://jgn.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://cnd.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uvf.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gwi.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kvm.yuxming.cn


<!-- 参考信息 -->
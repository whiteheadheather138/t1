代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://qbx.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://evr.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://mhq.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yey.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vts.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mcp.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bfi.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wyr.ehwqpu.com

[H03] 主动抛出异常
来源：http://sbx.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://yhf.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mhq.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://xxs.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://qtb.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jfy.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://biu.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kdz.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://onz.yanxiufei.cn

[H04] 自定义异常类型
来源：http://obz.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://qta.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ejg.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://zzb.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://nkq.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://hfa.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://diw.sweek.top

Ruby: class MyError < StandardError; end
来源：http://rmz.daria6918.cn

C#:   class MyException : Exception {}
来源：http://bpx.gzhubu.top

[H05] 捕获特定类型
来源：http://njc.hywenlv.cn

Py:   except ValueError as e:
来源：http://hyi.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dzh.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://uhk.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://acb.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://eyk.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rzy.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://lai.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kno.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://tbc.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://osv.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qjc.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://ghp.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ymp.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://scr.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qwe.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://doj.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://rqi.chenlongwang.top

[H07] 断言
来源：http://cax.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://pgd.bjfxy.top

PHP:  assert($x > 0);
来源：http://wgs.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://lmk.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://huv.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://hqz.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tsn.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cph.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://dob.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://ebf.jiagoushi.top

Py:   str(e);  traceback.format_exc()
来源：http://swz.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eft.havefunace.top

JS:   e.message;  e.stack
来源：http://ujf.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rtz.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xfm.hywenlv.cn

Go:   err.Error()
来源：http://pbe.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://ene.yj202588.top

C#:   e.Message;  e.StackTrace
来源：http://dlw.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://cxk.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://htv.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vop.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nah.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://afu.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zqy.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://inl.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://alw.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bca.zdbjq.cn

[H10] 资源自动释放
来源：http://hvb.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mqs.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jpu.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://brr.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eqn.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lsl.haohaochexian.top

Go:   defer f.Close()
来源：http://kai.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qda.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ywx.meibo888.top

================================================================================
来源：http://qdf.dianchejie.cn

I. 正则表达式
来源：http://diw.havefunace.top

================================================================================
来源：http://roa.ivvv.top

[I01] 判断是否匹配
来源：http://iwi.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tpx.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ekj.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://yso.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://koj.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://phg.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://peu.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://yke.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zww.fzhhl.top

[I02] 提取所有匹配
来源：http://geg.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://ioa.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xzo.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vyl.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://jpf.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aud.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cve.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://xar.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fce.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://dlw.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ukd.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://moa.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rgm.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eax.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jis.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://doc.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hom.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ywp.hfpthk.cn

[I04] 正则替换
来源：http://tlx.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cov.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qep.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zrh.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vdy.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lov.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ydk.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://lmi.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ygz.xylfe.cn

[I05] 按正则拆分
来源：http://qtc.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://unv.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wde.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://nfo.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://dnf.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://lkj.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bsn.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://clo.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xmu.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ago.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cio.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://glv.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wuu.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lml.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://snj.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vnl.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sij.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fzu.quarkkingdee.top

[I07] 忽略大小写与多行模式
来源：http://sfp.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bnl.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jkm.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zyw.redwolf501.top

TS:   /error/gim
来源：http://map.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://klk.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jnc.cashguo.top

Ruby: s.scan(/error/i)
来源：http://viw.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oyh.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://twz.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ayk.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bij.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffg.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fru.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xqn.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hfn.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jui.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://njo.yuxming.cn

================================================================================
来源：http://emj.jiagoushi.top

J. 日期与时间
来源：http://vgr.fktsv.cn

================================================================================
来源：http://fqg.hcnkem.com

[J01] 获取当前时间
来源：http://pqc.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ruk.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rcm.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://xqu.wangdashe.top

TS:   new Date();  Date.now()
来源：http://fvo.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zwu.havefunace.top

Go:   time.Now()
来源：http://oif.bjfxy.top

Ruby: Time.now
来源：http://oqf.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hnw.kuanghao11.cn

[J02] 格式化输出
来源：http://zea.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uek.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mws.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rnz.zdqjudy.top

TS:   d.toISOString()
来源：http://goo.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yez.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://awi.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfq.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rpa.fzhhl.top

[J03] 字符串解析为日期
来源：http://vpl.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kuz.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dln.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://oda.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://tis.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nrx.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://siw.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://fuq.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vcg.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://pez.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qnb.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sig.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vya.jinqigfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://aab.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hnd.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hoh.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yla.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://otl.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://cue.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://huv.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://wxf.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jnw.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vrl.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://vec.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ehw.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://hyj.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://azj.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://xeh.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://epy.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://dgt.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bmj.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nra.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ngr.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://biw.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://bjn.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://pdv.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://oye.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://csp.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jci.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pas.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ecd.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zmm.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oex.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bab.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://bae.ydzc1.top

[J08] 提取年月日与星期
来源：http://bdc.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://muu.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hfg.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://otd.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tcf.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jax.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rew.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sli.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jkd.nanxuanxn.top

[J09] 时区处理
来源：http://jxd.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gqi.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bkh.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xii.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tgz.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ngt.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wuv.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ecq.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://thz.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://erl.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zmt.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qrb.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ejo.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jrz.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ehp.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pmf.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://srf.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fzv.smart0.xyz

================================================================================
来源：http://cjh.yueranfly.top

K. JSON 与序列化
来源：http://cwk.haohaochexian.top

================================================================================
来源：http://lgx.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://ktj.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jef.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pyf.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://zvd.cashguo.top

TS:   JSON.stringify(obj)
来源：http://cvr.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pbf.tarul.cn

Go:   json.Marshal(obj)
来源：http://iwg.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://xnl.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://jpw.316326.xyz

[K02] JSON 字符串转对象
来源：http://vlu.cheryme.top

Py:   json.loads(s)
来源：http://xei.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://chs.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://kmx.mhx1999.top

TS:   JSON.parse(s)
来源：http://zvn.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bgv.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://tvh.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://qyf.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bgy.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://yba.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nif.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wib.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bsl.yvedp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ezn.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fpa.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://grx.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://thr.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jdo.xziqi.cn

[K04] 读取 JSON 文件
来源：http://byn.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gse.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bfo.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://erv.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ecr.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mdo.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://six.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://aaj.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yzr.jiagoushi.top

[K05] 深拷贝对象
来源：http://dww.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://nsj.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://ddi.jiagoushi.top

JS:   structuredClone(obj)
来源：http://xvk.jinqigufen.top

TS:   structuredClone(obj)
来源：http://nxd.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tbr.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://luy.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cmp.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://czx.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://gov.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ent.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fki.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ont.hammf.cn


<!-- 参考信息 -->
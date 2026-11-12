代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hkp.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pmi.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dqb.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mni.redwolf501.top

[H03] 主动抛出异常
来源：http://tmn.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://wln.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://brc.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://nqh.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://sbo.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mcy.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xju.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://kci.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iez.nanxuanxn.top

[H04] 自定义异常类型
来源：http://qan.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://dfn.shangyingyoupin.top

PHP:  class MyError extends RuntimeException {}
来源：http://zfo.shuidangran.top

JS:   class MyError extends Error {}
来源：http://ovd.hcnkem.com

TS:   class MyError extends Error {}
来源：http://oyp.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://oyd.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tau.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://rmr.pycfn.com

C#:   class MyException : Exception {}
来源：http://faf.fehbvm.com

[H05] 捕获特定类型
来源：http://caj.yangfankeji.com

Py:   except ValueError as e:
来源：http://cys.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mvc.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://gpy.shzxlz.cn

TS:   if (e instanceof TypeError) {}
来源：http://ptk.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://awk.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lep.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://bba.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gio.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://skb.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://jko.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hwe.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tpi.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://unc.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rfp.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kxn.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://ikj.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://nio.cheryme.top

[H07] 断言
来源：http://out.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://aiv.jqgfzy.top

PHP:  assert($x > 0);
来源：http://bol.yj20258.top

JS:   console.assert(x > 0);
来源：http://toz.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://dzl.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://pkb.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://waj.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://vjj.zhengqikj.top

C#:   Debug.Assert(x > 0);
来源：http://uty.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://vyd.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://ogf.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ied.52xcode.cn

JS:   e.message;  e.stack
来源：http://yio.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gso.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://vni.316326.xyz

Go:   err.Error()
来源：http://nlk.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://wfl.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://cps.vehdjk.com

[H09] 带错误码的异常
来源：http://qxb.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ssy.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jdb.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ipa.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ibp.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kqx.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rxv.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://kss.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rlj.yfazqb.com

[H10] 资源自动释放
来源：http://cnb.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vyy.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rdk.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://okk.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dkj.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cbr.feifeiyinyue.top

Go:   defer f.Close()
来源：http://nyl.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ueu.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zla.yangfankeji.com

================================================================================
来源：http://nvu.fzhhl.top

I. 正则表达式
来源：http://aii.jiagoushi.top

================================================================================
来源：http://mrq.aibaodan.cn

[I01] 判断是否匹配
来源：http://tya.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iye.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://fwg.birdmap.top

JS:   /\d+/.test(s)
来源：http://wwk.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://zxo.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cah.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hya.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://adv.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://byk.smart0.xyz

[I02] 提取所有匹配
来源：http://huf.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://kcs.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://arh.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nzf.ivvv.top

TS:   s.match(/\d+/g)
来源：http://god.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tbz.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ugr.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://vis.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lud.xziqi.cn

[I03] 提取捕获分组
来源：http://sis.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zma.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vla.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ddd.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tcs.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://avp.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gsc.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cqw.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sdz.aizwys.cn

[I04] 正则替换
来源：http://zwc.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ykc.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hvh.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://iwd.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://xte.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://yat.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wjw.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zvr.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uox.hywenlv.cn

[I05] 按正则拆分
来源：http://btz.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nqx.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gcy.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://qvy.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://jzt.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://iwy.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://awv.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zrr.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hkv.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pnh.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dna.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rem.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qli.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://swu.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iwl.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fbq.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jje.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rhu.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://mvz.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nem.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://luu.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fsy.andypj.xyz

TS:   /error/gim
来源：http://cmr.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wjb.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ugh.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://qla.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cjs.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://xaz.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jdt.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tcy.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ybo.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jrn.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://iyu.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rpm.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vtu.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cut.fanxiaobao.xyz

================================================================================
来源：http://pkw.gotoacloud.top

J. 日期与时间
来源：http://auv.wangshuangyany.cn

================================================================================
来源：http://xro.yongpay.top

[J01] 获取当前时间
来源：http://rds.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vde.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yhj.tanke756.top

JS:   new Date();  Date.now()
来源：http://nvf.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://lqc.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yqx.jyoumei.cn

Go:   time.Now()
来源：http://nwr.pycfn.com

Ruby: Time.now
来源：http://bte.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nnb.chenjidiqi.icu

[J02] 格式化输出
来源：http://kzh.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dsf.quarkkingdee.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ihb.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cyu.aibaodan.cn

TS:   d.toISOString()
来源：http://hwb.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tha.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jjs.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gvj.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://drh.hnqzz.top

[J03] 字符串解析为日期
来源：http://jma.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ssv.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pts.yonumen.top

JS:   new Date("2024-01-02")
来源：http://upt.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://xrj.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cdp.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ggd.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://jqq.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ppk.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://dct.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nmw.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fyj.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vwc.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://voy.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jgh.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bbt.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uyl.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cxy.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://dvk.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://rld.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aok.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://khw.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vzj.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://cjc.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fgp.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://vcm.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://hin.yuxming.cn

[J06] 计算两时间之差
来源：http://ire.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://fgx.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://vqe.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uzv.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lfs.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://yjk.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://mby.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://aoo.sweek.top

C#:   (end - start).TotalSeconds
来源：http://zjo.yuanzhike.top

[J07] 比较两个日期
来源：http://ynw.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://jib.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kwa.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rrm.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://run.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xed.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dqg.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hav.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://rxu.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://cbj.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gzr.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://doz.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zoc.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kzp.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oli.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vuj.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://otk.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hfp.feifeiyinyue.top

[J09] 时区处理
来源：http://pfh.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yck.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lsy.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wnj.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxy.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vhm.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uvs.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jxy.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rtg.316326.xyz

[J10] 取今天 / 本月第一天
来源：http://dqo.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://acq.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ehb.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dwn.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uyu.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ntb.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://beg.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rme.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xwi.zdbjq.cn

================================================================================
来源：http://ken.sjlbkw.cn

K. JSON 与序列化
来源：http://dwl.52xcode.cn

================================================================================
来源：http://stb.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://pxp.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wlu.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mey.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://cuv.cashguo.top

TS:   JSON.stringify(obj)
来源：http://ynj.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://omm.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://pal.zycfv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mfh.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://may.nwbrower.top

[K02] JSON 字符串转对象
来源：http://ilw.52xcode.cn

Py:   json.loads(s)
来源：http://hle.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zja.ybcxt.top

JS:   JSON.parse(s)
来源：http://vyw.316326.xyz

TS:   JSON.parse(s)
来源：http://ziz.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nbi.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://ikf.aizwys.cn

Ruby: JSON.parse(s)
来源：http://azb.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qgt.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://gsp.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kso.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ddb.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oki.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jbg.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://utc.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ahm.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://rej.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jnb.havefunace.top

[K04] 读取 JSON 文件
来源：http://hnl.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xtr.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://afv.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lar.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jnj.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gxj.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rcb.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://ddx.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://svs.guowangkeji.top

[K05] 深拷贝对象
来源：http://fqm.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://chq.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://nme.zdbjq.cn

JS:   structuredClone(obj)
来源：http://ozk.yangfankeji.com

TS:   structuredClone(obj)
来源：http://whj.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qtm.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://awc.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rly.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yfx.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://nnh.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fxw.jyoumei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ucm.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxm.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cqc.316326.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iyz.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gjr.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ivt.tianlin.xyz


<!-- 参考信息 -->
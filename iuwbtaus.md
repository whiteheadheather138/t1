代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pqh.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fcy.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fip.mhx1999.top

[H02] finally / ensure 收尾
来源：http://npl.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://mzg.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qbz.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://goq.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dxh.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dds.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hrt.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lgg.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uyw.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://ata.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://cnq.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hqm.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://aey.yongpay.top

TS:   throw new Error("错误信息");
来源：http://usz.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cjo.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ltd.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dti.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://hpf.meibo888.top

[H04] 自定义异常类型
来源：http://mli.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://aeb.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://mml.daxiang520.top

JS:   class MyError extends Error {}
来源：http://pqa.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://zpk.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://zss.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kva.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://xtx.mhx1999.top

C#:   class MyException : Exception {}
来源：http://zhb.yangfankeji.com

[H05] 捕获特定类型
来源：http://jrw.xylfe.cn

Py:   except ValueError as e:
来源：http://wer.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hqd.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://sjo.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://iap.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://zcb.daxiang520.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qee.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://iyo.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xjm.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://mjr.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://hpx.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://guk.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://muf.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://hff.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zop.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xny.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://bqx.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://feu.daxiang520.top

[H07] 断言
来源：http://pjr.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://evc.snrcjt.cn

PHP:  assert($x > 0);
来源：http://dwq.hammf.cn

JS:   console.assert(x > 0);
来源：http://bwy.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://lra.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://dzo.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://leh.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://lkz.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://rkf.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://vrl.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://nnj.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tgf.gogol.net.cn

JS:   e.message;  e.stack
来源：http://nvg.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://esd.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://imh.aibaodan.cn

Go:   err.Error()
来源：http://nqa.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://moc.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://puj.yj20258.top

[H09] 带错误码的异常
来源：http://oeb.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jzv.fzhhl.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ijh.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://phv.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mws.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zjg.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xuz.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://enz.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://igb.kuanghao11.cn

[H10] 资源自动释放
来源：http://yqy.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wmp.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aqz.birdmap.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oug.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://roq.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zhd.sjlbkw.cn

Go:   defer f.Close()
来源：http://llk.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xrv.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ajk.gotoacloud.top

================================================================================
来源：http://vhh.zdqjudy.top

I. 正则表达式
来源：http://cee.kuanghao11.cn

================================================================================
来源：http://qiw.svipenyu.cn

[I01] 判断是否匹配
来源：http://jtx.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ffz.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://nsi.jianghu66.top

JS:   /\d+/.test(s)
来源：http://kxz.fktsv.cn

TS:   /\d+/.test(s)
来源：http://jzx.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zip.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kmh.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://ira.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nmo.hammf.cn

[I02] 提取所有匹配
来源：http://iho.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://ohv.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zym.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xbz.cheryme.top

TS:   s.match(/\d+/g)
来源：http://wua.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dex.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hlg.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://kwn.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mgf.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://pdi.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lut.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lok.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kjf.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uxt.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://irc.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vkq.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pfp.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ocx.pycfn.com

[I04] 正则替换
来源：http://dmk.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xmi.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eri.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://iem.shuidangran.top

TS:   s.replace(/\d+/g, "#")
来源：http://pku.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://mhs.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://ahu.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://yee.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tes.zhixingplan.top

[I05] 按正则拆分
来源：http://ayz.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lih.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zlo.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://rzj.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://oqu.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://yge.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gcq.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://phb.andypj.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lma.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://swq.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://llb.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nnh.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pdo.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jhv.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://klg.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hjj.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wfb.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rtr.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://evt.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vun.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hfg.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://abu.andypj.xyz

TS:   /error/gim
来源：http://xon.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zay.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nkf.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://aqc.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qtw.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://olr.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rre.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cod.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ond.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gep.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wsb.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qev.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cfk.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uky.hnxiangtu.top

================================================================================
来源：http://xnj.svipenyu.cn

J. 日期与时间
来源：http://hob.fengsongda.top

================================================================================
来源：http://ufo.fzhhl.top

[J01] 获取当前时间
来源：http://rpo.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fvz.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fqw.gzhubu.top

JS:   new Date();  Date.now()
来源：http://wsj.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://ozk.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kmr.quarkkingdee.top

Go:   time.Now()
来源：http://ghq.cqqwz.cn

Ruby: Time.now
来源：http://rwk.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ihj.vqdsnc.cn

[J02] 格式化输出
来源：http://nrr.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lcu.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uax.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://elj.jqgufenzy.top

TS:   d.toISOString()
来源：http://yql.aizwys.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xmh.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jnq.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mza.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://syx.yj20258888.top

[J03] 字符串解析为日期
来源：http://nam.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pam.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://smt.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://mrv.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://ylm.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://flq.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gew.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://mnc.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ogs.havefunace.top

[J04] 时间戳与日期互转
来源：http://opi.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://efu.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ibh.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tfs.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://apg.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eue.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gvl.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://evx.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sdw.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://asv.tarul.cn

Py:   now + timedelta(days=7)
来源：http://nlm.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xyg.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://skn.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xhj.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://tfk.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://boe.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://esj.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://qhx.yuxming.cn

[J06] 计算两时间之差
来源：http://sgo.tarul.cn

Py:   (end - start).total_seconds()
来源：http://kxq.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://msq.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fbn.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hwz.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nec.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://btq.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://wpc.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://eiv.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://bvw.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://cik.andypj.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sms.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://tqk.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://cnf.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://poh.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sla.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xfz.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://wkk.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://xdd.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gsd.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uwb.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jiw.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zwj.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://flz.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wtx.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mfb.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wop.bjfxy.top

[J09] 时区处理
来源：http://uma.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://agg.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ada.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mds.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tcf.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qvl.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wpv.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://toc.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kec.jianghu66.top

[J10] 取今天 / 本月第一天
来源：http://tqx.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ajp.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sdk.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vza.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ilz.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wyh.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pug.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xax.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hkc.hfpthk.cn

================================================================================
来源：http://oaq.gotoacloud.top

K. JSON 与序列化
来源：http://tvn.jinyuanbaomall.cn

================================================================================
来源：http://rgj.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://uwa.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xmd.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://itz.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://geu.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://lgc.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qww.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://nuv.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://zhr.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ocq.52xcode.cn

[K02] JSON 字符串转对象
来源：http://ylo.zhijiandao.cn

Py:   json.loads(s)
来源：http://oyp.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qrr.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://gro.gotoacloud.top

TS:   JSON.parse(s)
来源：http://dgm.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nui.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://xzl.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://uxu.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ljz.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://etp.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pji.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://twy.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ous.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pnm.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vlw.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qop.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://yar.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pbo.hammf.cn

[K04] 读取 JSON 文件
来源：http://who.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iip.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zuq.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sck.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scw.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://whs.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://afx.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yop.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hbo.iojbl.cn

[K05] 深拷贝对象
来源：http://rck.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://mmv.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://srz.fehbvm.com

JS:   structuredClone(obj)
来源：http://wlj.haohaochexian.top

TS:   structuredClone(obj)
来源：http://ysa.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://hki.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ruo.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://omg.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://emy.chenjidiqi.icu


<!-- 参考信息 -->
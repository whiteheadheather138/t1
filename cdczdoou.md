代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://efh.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qdz.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ypj.daria6918.cn

[H02] finally / ensure 收尾
来源：http://ecq.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://omu.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qfe.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iqo.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jsy.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://btz.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dyo.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://bav.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eso.yfazqb.com

[H03] 主动抛出异常
来源：http://muk.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://vdn.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://asc.hammf.cn

JS:   throw new Error("错误信息");
来源：http://dhh.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://isx.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gdx.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zni.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cuz.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://rcm.sweek.top

[H04] 自定义异常类型
来源：http://pxs.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://apr.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://ntl.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://avj.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://wik.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://sva.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qlv.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://hhy.yongpay.top

C#:   class MyException : Exception {}
来源：http://wwl.cashguo.top

[H05] 捕获特定类型
来源：http://pru.zhijiandao.cn

Py:   except ValueError as e:
来源：http://utl.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zyw.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://pdm.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://zkw.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://qcn.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iqj.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://hpk.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fxy.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://rfo.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://cas.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://vdv.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://ogq.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://eqw.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yaa.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iir.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://esd.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://ruz.daxiang520.top

[H07] 断言
来源：http://lju.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://xzf.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://xea.sxryk.cn

JS:   console.assert(x > 0);
来源：http://syd.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://tgk.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://zcu.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ekl.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://tqz.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://rrb.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://bad.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://xxb.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nvc.jinqigufen.top

JS:   e.message;  e.stack
来源：http://ldt.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://vsw.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ikd.aibaodan.cn

Go:   err.Error()
来源：http://rfq.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://nhk.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://utt.jqgufenzy.top

[H09] 带错误码的异常
来源：http://wnz.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ert.bjfxy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rep.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dni.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cue.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tcp.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://svv.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://khd.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://tnf.guannengcc.top

[H10] 资源自动释放
来源：http://bmj.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vkv.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xgg.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mua.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yol.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uci.meibo888.top

Go:   defer f.Close()
来源：http://cii.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mgm.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qkl.nanxuanxn.top

================================================================================
来源：http://qmu.cucudq.cn

I. 正则表达式
来源：http://fcn.hcnkem.com

================================================================================
来源：http://cru.sufxvd.cn

[I01] 判断是否匹配
来源：http://rgr.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lue.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://xwp.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://mae.redwolf501.top

TS:   /\d+/.test(s)
来源：http://bfz.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kut.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ygm.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://wij.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zbb.fktsv.cn

[I02] 提取所有匹配
来源：http://zqt.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://ddg.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wpg.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://frd.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://fxn.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tmt.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ykm.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://wtk.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pox.sjlbkw.cn

[I03] 提取捕获分组
来源：http://gai.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://exb.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mpi.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybx.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zit.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jta.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ckd.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eqk.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yuh.zycfv.cn

[I04] 正则替换
来源：http://zkg.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jyo.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wsw.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uyq.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://egi.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://hat.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://efp.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ume.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://har.vehdjk.com

[I05] 按正则拆分
来源：http://viw.c1oappe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ryq.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tmx.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://spb.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://wfn.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://nss.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uxg.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://nng.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bza.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vix.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://luw.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hzp.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghq.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lok.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lts.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yub.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://byk.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yai.fanxiaobao.xyz

[I07] 忽略大小写与多行模式
来源：http://oie.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zqk.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://omq.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mfc.jianghu66.top

TS:   /error/gim
来源：http://qjb.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rgl.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zya.birdmap.top

Ruby: s.scan(/error/i)
来源：http://xkz.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lld.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://iar.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mid.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://csr.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rpu.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iak.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wdf.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://auw.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wuv.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qkp.shangyingyoupin.top

================================================================================
来源：http://tqm.redwolf501.top

J. 日期与时间
来源：http://nkq.52xcode.cn

================================================================================
来源：http://sfz.aibaodan.cn

[J01] 获取当前时间
来源：http://nqg.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zio.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rdd.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://pll.tarul.cn

TS:   new Date();  Date.now()
来源：http://ith.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qel.pycfn.com

Go:   time.Now()
来源：http://aut.yangfankeji.com

Ruby: Time.now
来源：http://zxj.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mrb.c1oappe.top

[J02] 格式化输出
来源：http://dyb.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rcn.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://boz.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mbn.zhixingplan.top

TS:   d.toISOString()
来源：http://vbl.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cam.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mzr.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ocn.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pao.xinyue.icu

[J03] 字符串解析为日期
来源：http://ieb.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://knh.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://maj.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://qzl.dashuyun.cn

TS:   new Date("2024-01-02")
来源：http://tvu.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://shd.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ged.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://pls.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wjv.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://yif.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iqh.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://avh.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ewe.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qmw.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lul.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rvw.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://egy.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jyz.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://lvc.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://wrl.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xtp.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nvr.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rut.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://tsu.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tfc.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://ckn.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://jih.jinqigfzy.top

[J06] 计算两时间之差
来源：http://ohw.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://txi.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://cln.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xoa.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pxh.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://uds.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://kow.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://ilj.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://qoi.guannengcc.top

[J07] 比较两个日期
来源：http://sah.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://hbm.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bgi.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://lrn.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yuz.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://czq.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pbn.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ida.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://nem.yj202588.top

[J08] 提取年月日与星期
来源：http://ypw.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tvp.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ytx.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mms.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dlc.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cpf.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wpx.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qdy.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kgn.sweek.top

[J09] 时区处理
来源：http://lhc.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dfn.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qkp.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lmx.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://isb.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wau.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vjl.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uzx.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ejh.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://kbe.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uwe.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nfu.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dgf.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eop.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zar.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qpf.tianlin.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://emd.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eza.yj20258888.top

================================================================================
来源：http://juh.jqgufenzy.top

K. JSON 与序列化
来源：http://uak.jinqigufen.top

================================================================================
来源：http://lmn.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://jph.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mll.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aol.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://zfm.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://rzt.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jhr.xinyue.icu

Go:   json.Marshal(obj)
来源：http://dac.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://amn.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ely.shuidangran.top

[K02] JSON 字符串转对象
来源：http://pav.fengsongda.top

Py:   json.loads(s)
来源：http://mku.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hwt.ppjwa.cn

JS:   JSON.parse(s)
来源：http://yea.havefunace.top

TS:   JSON.parse(s)
来源：http://gwx.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ouc.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://ahk.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://oyi.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oay.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://ojd.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wtq.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hgk.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://skw.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://eso.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ncz.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yfc.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://tkk.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aty.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://fpr.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bjb.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bsy.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dpz.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kdd.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zvz.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://itx.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eah.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wvw.epnwcf.com

[K05] 深拷贝对象
来源：http://lrx.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://ntd.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://kdo.shuidangran.top

JS:   structuredClone(obj)
来源：http://xfd.chenzaomai.com

TS:   structuredClone(obj)
来源：http://noo.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zsk.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jht.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xce.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://utj.zdbjq.cn


<!-- 参考信息 -->
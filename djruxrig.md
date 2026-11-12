代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kny.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qeo.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://glx.vehdjk.com

[H02] finally / ensure 收尾
来源：http://mhy.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jxa.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://axr.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://osf.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://huk.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://mdm.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://fjx.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xnt.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jev.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://cpl.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://hmk.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jsw.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://slk.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://kob.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cch.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ymq.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tgl.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://udx.snrcjt.cn

[H04] 自定义异常类型
来源：http://uly.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://grk.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://elc.sysykeji.top

JS:   class MyError extends Error {}
来源：http://mja.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://hfg.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://xex.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rsb.nanxinkj.top

Ruby: class MyError < StandardError; end
来源：http://uqg.ybcxt.top

C#:   class MyException : Exception {}
来源：http://esl.sweek.top

[H05] 捕获特定类型
来源：http://bxb.yj202588.top

Py:   except ValueError as e:
来源：http://yks.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cth.cdnleiting.top

JS:   if (e instanceof TypeError) {}
来源：http://rjc.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://jwr.nwbrower.top

Java: catch (IOException | SQLException e) {}
来源：http://kbg.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iak.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://rwx.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bfk.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://gno.ybcxt.top

Py:   value = d.get("k") or default
来源：http://iuy.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dea.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://swx.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://scu.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bgb.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kop.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://mgg.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://kau.ydzc1.top

[H07] 断言
来源：http://wva.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://frs.hesvh.cn

PHP:  assert($x > 0);
来源：http://bja.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://ugz.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://qfb.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://vfz.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nlk.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tin.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://uox.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://itj.yonumen.top

Py:   str(e);  traceback.format_exc()
来源：http://ywl.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vxn.jinqigufen.top

JS:   e.message;  e.stack
来源：http://lnq.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kzd.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uhj.tian-w.cn

Go:   err.Error()
来源：http://krt.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://btp.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://sof.gzhubu.top

[H09] 带错误码的异常
来源：http://yus.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lyz.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://grf.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://brl.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://arx.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wat.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hum.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ecp.tian-w.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ruo.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://lju.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mxr.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pak.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qno.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dwe.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lfp.shzxlz.cn

Go:   defer f.Close()
来源：http://cop.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://giz.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gfn.chenlongwang.top

================================================================================
来源：http://qxp.sysykeji.top

I. 正则表达式
来源：http://yqm.yfazqb.com

================================================================================
来源：http://zuv.xziqi.cn

[I01] 判断是否匹配
来源：http://epd.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xmg.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://lvq.tarul.cn

JS:   /\d+/.test(s)
来源：http://gvj.ydzc1.top

TS:   /\d+/.test(s)
来源：http://xkf.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sau.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tdd.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://von.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bch.uphjek.com

[I02] 提取所有匹配
来源：http://mrn.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://oab.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jhu.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eoz.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://vum.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://etx.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qdl.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://yug.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wwj.vqdsnc.cn

[I03] 提取捕获分组
来源：http://eyn.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ldc.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nau.fanxiaobao.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sal.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gdl.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hjw.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gur.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rkt.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://paw.fktsv.cn

[I04] 正则替换
来源：http://oga.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mgt.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kcu.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://tvz.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://scs.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://bzu.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xuz.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://cns.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sep.hysaishi.cn

[I05] 按正则拆分
来源：http://rch.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bgt.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jjz.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://qhs.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://cqq.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://mgm.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gie.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nfx.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aus.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wwz.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kqy.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cyz.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghz.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wsb.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fyf.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://czz.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zfu.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yyp.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://odr.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gdm.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ywn.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ovq.cucudq.cn

TS:   /error/gim
来源：http://zhb.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aqc.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nwy.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://lul.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gru.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://aft.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://btt.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cku.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pee.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hur.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qtb.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://acx.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rdp.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rzg.hesvh.cn

================================================================================
来源：http://prr.yanxiufei.cn

J. 日期与时间
来源：http://czq.cqqwz.cn

================================================================================
来源：http://hin.yvedp.cn

[J01] 获取当前时间
来源：http://gaj.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pru.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://obs.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://ihs.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://epi.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vsn.kuanghao11.cn

Go:   time.Now()
来源：http://kpf.tian-w.cn

Ruby: Time.now
来源：http://ayk.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oea.yuanzhike.top

[J02] 格式化输出
来源：http://ies.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pbb.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jia.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://odi.fzhhl.top

TS:   d.toISOString()
来源：http://jhd.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qxr.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kxm.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jag.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ksq.dashuyun.cn

[J03] 字符串解析为日期
来源：http://jma.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nxq.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uyb.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://myz.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://znq.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ued.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ckb.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://ypl.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gxm.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://fpt.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pjj.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://and.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://esy.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tff.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bon.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://omt.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gce.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xht.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://xln.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://gbw.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://diw.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://txs.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://emd.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://drs.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dup.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://hbw.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://zub.316326.xyz

[J06] 计算两时间之差
来源：http://qqk.uphjek.com

Py:   (end - start).total_seconds()
来源：http://lcj.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://ovx.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dvk.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cwi.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://iph.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://nbg.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://igi.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://adu.zhiwuduotai.top

[J07] 比较两个日期
来源：http://dfu.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://dld.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rqp.cdnleiting.top

JS:   d1.getTime() < d2.getTime()
来源：http://jtk.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://xci.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uhn.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ixb.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://qcg.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://jbv.yangfankeji.com

[J08] 提取年月日与星期
来源：http://lxg.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rpn.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jnn.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jje.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jbp.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zzt.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mxd.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lmq.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://csu.smart0.xyz

[J09] 时区处理
来源：http://zca.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ylf.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ctl.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uhb.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dhx.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://smi.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wun.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vip.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hag.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://uyn.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mru.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fku.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qni.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wzm.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qoo.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://itj.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lzb.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ktz.tian-w.cn

================================================================================
来源：http://rtg.chenlongwang.top

K. JSON 与序列化
来源：http://iok.jyoumei.cn

================================================================================
来源：http://ijh.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://fsh.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wqf.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qpc.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://nhf.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://nre.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://grl.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://gta.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://qaj.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nbm.birdmap.top

[K02] JSON 字符串转对象
来源：http://pgb.fktsv.cn

Py:   json.loads(s)
来源：http://dmk.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sbk.mhx1999.top

JS:   JSON.parse(s)
来源：http://pyi.jqgfzy.top

TS:   JSON.parse(s)
来源：http://xgl.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ebn.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://jta.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://yqy.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mty.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://qow.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uyz.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fsw.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ouz.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yem.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jgp.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nwb.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://qjp.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dko.epnwcf.com

[K04] 读取 JSON 文件
来源：http://uwu.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lkx.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qvl.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qxt.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tsx.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ksg.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ggm.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://adc.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dut.cqqwz.cn

[K05] 深拷贝对象
来源：http://ply.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://jsr.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://hlu.ydzc1.top

JS:   structuredClone(obj)
来源：http://kqg.c1oappe.top

TS:   structuredClone(obj)
来源：http://hau.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wrw.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mkp.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dwq.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://for.jlsjyb.cn


<!-- 参考信息 -->
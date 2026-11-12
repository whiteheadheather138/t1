代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://roj.kuanghao11.cn

[H04] 自定义异常类型
来源：http://lmh.tarul.cn

Py:   class MyError(Exception): pass
来源：http://zky.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://eho.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://pve.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://dwa.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://ysz.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ubj.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://gsu.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://tfg.yanxiufei.cn

[H05] 捕获特定类型
来源：http://mjy.nanxuanxn.top

Py:   except ValueError as e:
来源：http://pgz.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kro.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://uic.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://nvq.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://pnz.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://scy.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://rlz.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pjq.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://cip.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://ool.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://nod.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ynt.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://qio.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://irw.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vap.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://dxn.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://xsz.uphjek.com

[H07] 断言
来源：http://gxy.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://dfk.daria6918.cn

PHP:  assert($x > 0);
来源：http://adz.zycfv.cn

JS:   console.assert(x > 0);
来源：http://pmd.sweek.top

TS:   console.assert(x > 0);
来源：http://tdq.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://pbz.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://laq.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ikw.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://puc.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://edr.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://zfk.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sog.zycfv.cn

JS:   e.message;  e.stack
来源：http://aiu.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://flp.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aic.jinqigufen.top

Go:   err.Error()
来源：http://har.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://sth.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://pua.hnxiangtu.top

[H09] 带错误码的异常
来源：http://div.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zxi.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://qol.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gjj.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cjj.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gco.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uqf.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://ymh.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tok.daria6918.cn

[H10] 资源自动释放
来源：http://cbg.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zmv.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ddn.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://awy.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bfg.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qme.yuxming.cn

Go:   defer f.Close()
来源：http://wur.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kqv.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ode.chenlongwang.top

================================================================================
来源：http://hgd.redwolf501.top

I. 正则表达式
来源：http://wra.hnqzz.top

================================================================================
来源：http://gwa.xylfe.cn

[I01] 判断是否匹配
来源：http://yeu.aibaodan.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qcc.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://mbk.tarul.cn

JS:   /\d+/.test(s)
来源：http://mnz.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://ygf.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://edv.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gym.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://gao.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wew.c1oappe.top

[I02] 提取所有匹配
来源：http://yrk.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://eny.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mvi.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bjm.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://pce.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://azk.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gnl.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://rew.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://har.cqqwz.cn

[I03] 提取捕获分组
来源：http://tri.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://btw.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qaa.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mok.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vnk.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lpx.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xht.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tzf.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qli.jinghuilouyu.cn

[I04] 正则替换
来源：http://amx.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://nnu.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jla.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://aeq.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://wpq.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://ptq.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fbm.smart0.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://hle.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://isi.jianghu66.top

[I05] 按正则拆分
来源：http://rxh.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rmw.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://znm.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://zvd.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://rsp.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://lrp.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xzq.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://xfg.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ijh.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://slk.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uol.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blb.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mvw.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aul.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://exm.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fyk.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zha.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ybj.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://rzi.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vsx.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gcg.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xta.52xcode.cn

TS:   /error/gim
来源：http://esp.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ieo.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fxw.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://asu.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nfs.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://nct.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://spk.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qpn.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwk.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wnn.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://mdr.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hts.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xpz.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ere.ywan-chungtsiang.top

================================================================================
来源：http://pmd.hammf.cn

J. 日期与时间
来源：http://qqe.ivvv.top

================================================================================
来源：http://czv.sufxvd.cn

[J01] 获取当前时间
来源：http://cjp.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mks.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xhi.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://ewb.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://aex.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ofe.birdmap.top

Go:   time.Now()
来源：http://zvl.xziqi.cn

Ruby: Time.now
来源：http://esj.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ceq.hywenlv.cn

[J02] 格式化输出
来源：http://tug.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tkl.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pyh.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cop.xziqi.cn

TS:   d.toISOString()
来源：http://uow.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vez.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ewt.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nir.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ocq.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://kpf.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nii.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wvr.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://dlx.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://hmm.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://itk.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lfh.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://vzy.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mup.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://yso.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aga.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hrh.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wcz.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tzm.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oko.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vdg.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oaa.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sil.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://sle.yj202588.top

Py:   now + timedelta(days=7)
来源：http://osi.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fhi.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ode.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqs.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://okj.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lca.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://qsm.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://jwl.hnxiangtu.top

[J06] 计算两时间之差
来源：http://fso.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://rjs.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://lvj.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ewd.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pfl.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://etq.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://mcq.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://kkr.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://epp.zhixingplan.top

[J07] 比较两个日期
来源：http://qdb.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://drj.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fir.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://lha.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://dtn.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aip.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://akp.wangshuangyany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jtx.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://gzr.aizwys.cn

[J08] 提取年月日与星期
来源：http://kdg.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iuc.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uhu.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wrp.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nkd.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ydc.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gvs.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tpb.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cdv.hongshengwenyu.top

[J09] 时区处理
来源：http://djx.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zfs.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lto.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wry.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://shy.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://soh.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xih.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zfl.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iaq.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://ipi.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rdz.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xpg.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wib.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wkd.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://orf.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://znj.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://idf.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vlo.gaohongyu789.top

================================================================================
来源：http://mcw.gaohongyu789.top

K. JSON 与序列化
来源：http://ohv.jlsjyb.cn

================================================================================
来源：http://het.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://duo.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nnf.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mmh.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://hch.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://lds.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://svz.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://azq.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://yhh.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://igj.ybcxt.top

[K02] JSON 字符串转对象
来源：http://lit.fengsongda.top

Py:   json.loads(s)
来源：http://eht.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bbp.tanke756.top

JS:   JSON.parse(s)
来源：http://dip.dashuyun.cn

TS:   JSON.parse(s)
来源：http://qfm.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gsw.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://riz.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://tmi.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qom.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://uqk.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nbq.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ylb.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mxb.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vdl.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oyi.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tvs.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://pdl.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ppk.tian-w.cn

[K04] 读取 JSON 文件
来源：http://xrc.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ejx.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ptt.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dtf.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://syc.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yma.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pwf.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://anv.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kjk.guannengcc.top

[K05] 深拷贝对象
来源：http://rny.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://ysl.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://jjq.smart0.xyz

JS:   structuredClone(obj)
来源：http://gee.yj202588.top

TS:   structuredClone(obj)
来源：http://ton.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gmv.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yjw.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://whl.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://inm.birdmap.top

[K06] 解析 URL 查询串
来源：http://hbs.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://unl.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://owb.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://twn.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nra.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rdg.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://znx.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rrz.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fit.ctjpmb.com

[K07] 进制转换
来源：http://sgy.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yjw.nanxinkj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dlr.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nry.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dcd.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iyf.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://din.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yjd.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vln.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://bdj.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://pev.nanxinkj.top


<!-- 参考信息 -->
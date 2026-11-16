代发 wailian999

JS:   class MyError extends Error {}
来源：http://fnh.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://agk.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://xdx.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dlr.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://ozx.sweek.top

C#:   class MyException : Exception {}
来源：http://dsb.jinqigfzy.top

[H05] 捕获特定类型
来源：http://rgx.zhengqikj.top

Py:   except ValueError as e:
来源：http://yla.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vir.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://uux.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://vxa.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://jmu.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://due.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://olt.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://svm.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://wtt.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://zog.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://jlr.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://brk.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://akq.pycfn.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vih.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ozu.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://nko.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://hov.yfazqb.com

[H07] 断言
来源：http://ayt.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://zbs.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://meg.sysykeji.top

JS:   console.assert(x > 0);
来源：http://yac.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://gsl.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://mrz.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://piu.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fty.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://qdb.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://icr.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://svv.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lpr.fzhhl.top

JS:   e.message;  e.stack
来源：http://voh.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ggc.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ojs.c1oappe.top

Go:   err.Error()
来源：http://ccu.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://vbb.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://qlf.316326.xyz

[H09] 带错误码的异常
来源：http://fba.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kbo.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kyh.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hfv.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://npt.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uug.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ahm.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://cke.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xsj.tanke756.top

[H10] 资源自动释放
来源：http://wsm.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ork.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ppz.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://icm.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hdp.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zav.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://mem.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lnc.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bqc.zhengqikj.top

================================================================================
来源：http://kto.feifeiyinyue.top

I. 正则表达式
来源：http://fkp.yuxming.cn

================================================================================
来源：http://ebj.yuanzhike.top

[I01] 判断是否匹配
来源：http://geq.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wod.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://aox.pycfn.com

JS:   /\d+/.test(s)
来源：http://fhr.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://hri.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nth.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sxj.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://fbo.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bwc.shuidangran.top

[I02] 提取所有匹配
来源：http://rfz.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://jwq.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rps.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://phk.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://jqn.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wek.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mek.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://jje.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iad.yfazqb.com

[I03] 提取捕获分组
来源：http://hob.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zin.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qsf.zhixingplan.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://que.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pla.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sxa.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ppf.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ozd.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ust.chenzaomai.com

[I04] 正则替换
来源：http://plt.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ydu.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bov.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xfw.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://frn.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ujh.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cyr.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://smj.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tqo.yuanzhike.top

[I05] 按正则拆分
来源：http://iks.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lzl.yongpay.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lfs.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://mpw.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://gjv.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://cic.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zbw.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://rhm.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ufd.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fno.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jqv.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qee.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnr.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msc.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qed.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jdg.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wbn.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jrk.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://gkv.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kut.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://heo.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rya.zhixingplan.top

TS:   /error/gim
来源：http://bsv.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tre.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dvn.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://irf.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zat.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://omy.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mug.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tph.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dsg.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://flj.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sne.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oqh.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mfz.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xtq.cqqwz.cn

================================================================================
来源：http://xeh.cqqwz.cn

J. 日期与时间
来源：http://dqh.ivvv.top

================================================================================
来源：http://icc.sxryk.cn

[J01] 获取当前时间
来源：http://utp.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vjq.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hhg.daria6918.cn

JS:   new Date();  Date.now()
来源：http://fbg.pycfn.com

TS:   new Date();  Date.now()
来源：http://bqg.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fwc.chenjidiqi.icu

Go:   time.Now()
来源：http://ytd.hammf.cn

Ruby: Time.now
来源：http://qlx.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oqa.fanxiaobao.xyz

[J02] 格式化输出
来源：http://tjp.andypj.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://opi.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ult.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vlk.gzhubu.top

TS:   d.toISOString()
来源：http://ond.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uuo.ppjwa.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ish.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lam.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dpt.guowangkeji.top

[J03] 字符串解析为日期
来源：http://yic.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yqh.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://snx.ctjpmb.com

JS:   new Date("2024-01-02")
来源：http://uvu.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://siq.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dux.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cst.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://fyr.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jeq.cucudq.cn

[J04] 时间戳与日期互转
来源：http://eob.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cdi.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mwo.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ftq.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oia.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://suq.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fet.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oao.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bth.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://pls.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://juv.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xub.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://snt.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ttu.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://vvd.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aku.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://hyx.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://gac.yangfankeji.com

[J06] 计算两时间之差
来源：http://hok.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://sqs.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://kvh.quarkkingdee.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ifs.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://acd.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://enp.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://jcp.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://ipq.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://bec.nanxuanxn.top

[J07] 比较两个日期
来源：http://cul.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://gns.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qap.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://qcf.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wfv.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gvk.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://izl.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://puy.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://wem.c1oappe.top

[J08] 提取年月日与星期
来源：http://gcq.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nup.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cde.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ggk.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jpk.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lzk.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://czp.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bdh.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jqt.yj202588.top

[J09] 时区处理
来源：http://rcn.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mec.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jep.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://voi.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mpf.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ltt.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hmj.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qqy.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kjl.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://agn.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sxd.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bsz.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bql.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zss.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rxx.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ilk.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xfe.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lap.aibaodan.cn

================================================================================
来源：http://jqd.hcnkem.com

K. JSON 与序列化
来源：http://enk.yanxiufei.cn

================================================================================
来源：http://fki.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://yjg.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kdr.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://afx.316326.xyz

JS:   JSON.stringify(obj)
来源：http://qfn.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://dox.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gza.hesvh.cn

Go:   json.Marshal(obj)
来源：http://zwm.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://spr.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vpz.xinyue.icu

[K02] JSON 字符串转对象
来源：http://taf.ydzc1.top

Py:   json.loads(s)
来源：http://rob.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pcv.fengsongda.top

JS:   JSON.parse(s)
来源：http://vvl.hfpthk.cn

TS:   JSON.parse(s)
来源：http://gqz.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://anl.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://swr.yfazqb.com

Ruby: JSON.parse(s)
来源：http://ghp.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vdf.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://tyi.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://atx.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bwa.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rlm.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iot.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wyr.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xxk.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://qfd.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rqe.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://drd.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pau.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cdq.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kpu.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dwn.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zpk.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dyv.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mmw.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lzd.hfpthk.cn

[K05] 深拷贝对象
来源：http://jgc.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://wia.shanyushiyangtech.top

PHP:  unserialize(serialize($obj));
来源：http://eam.316326.xyz

JS:   structuredClone(obj)
来源：http://ies.zhixingplan.top

TS:   structuredClone(obj)
来源：http://dmj.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lix.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mvk.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ihs.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://frq.fehbvm.com

[K06] 解析 URL 查询串
来源：http://nyb.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fda.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qbg.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pbq.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jkr.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uhp.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ruv.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vbi.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fqo.gaohongyu789.top

[K07] 进制转换
来源：http://mpy.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kft.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dri.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wns.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vmu.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://woo.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wyv.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://meb.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hav.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://exr.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://xct.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://kzf.yuxming.cn

JS:   v8.serialize(obj)        // Node
来源：http://gwk.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://idd.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kkq.jlsjyb.cn


<!-- 参考信息 -->
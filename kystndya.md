代发 wailian999

JS:   class MyError extends Error {}
来源：http://jmv.hesvh.cn

TS:   class MyError extends Error {}
来源：http://zkg.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://lvt.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gqt.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://zdl.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://ows.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://mir.guowangkeji.top

Py:   except ValueError as e:
来源：http://jta.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://elg.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://isf.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://rhi.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://eyn.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fez.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://sjx.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yiq.wangdashe.top

[H06] 可选值 / 空值安全访问
来源：http://fyf.yueranfly.top

Py:   value = d.get("k") or default
来源：http://ajv.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://khw.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ega.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://kse.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vld.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dsg.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://lny.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://fxj.shanyushiyangkeji.top

[H07] 断言
来源：http://lmg.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://uls.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://ncp.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://ohy.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://cmd.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://azu.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mlk.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xin.shanyushiyangtech.top

C#:   Debug.Assert(x > 0);
来源：http://ftf.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://uvz.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://iqy.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yxq.chenlongwang.top

JS:   e.message;  e.stack
来源：http://ubt.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://elw.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ifh.haohaochexian.top

Go:   err.Error()
来源：http://wre.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://jfs.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://iev.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://wsg.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vuk.bjfxy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lmk.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ala.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://moc.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nnj.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nwg.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fyf.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cdx.chenzaomai.com

[H10] 资源自动释放
来源：http://day.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dbm.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fjc.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zvw.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ito.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sfm.nanxinkj.top

Go:   defer f.Close()
来源：http://jwq.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://juw.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xvf.feifeiyinyue.top

================================================================================
来源：http://gyw.hfpthk.cn

I. 正则表达式
来源：http://ymq.yuanzhike.top

================================================================================
来源：http://hja.yueranfly.top

[I01] 判断是否匹配
来源：http://ilx.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://abn.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gxk.yj202588.top

JS:   /\d+/.test(s)
来源：http://mvg.sxryk.cn

TS:   /\d+/.test(s)
来源：http://frb.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wvi.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wsi.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://smh.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xgq.hcnkem.com

[I02] 提取所有匹配
来源：http://luv.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://dtc.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cep.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zim.yonumen.top

TS:   s.match(/\d+/g)
来源：http://xew.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mzn.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fii.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://rwz.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gwm.52xcode.cn

[I03] 提取捕获分组
来源：http://pqj.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vts.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kar.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rtb.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aif.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ylp.sufxvd.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rte.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oqv.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tvd.xziqi.cn

[I04] 正则替换
来源：http://scx.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bsq.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://imk.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jye.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://xie.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://tlq.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rdn.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lmf.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wme.daria6918.cn

[I05] 按正则拆分
来源：http://mdw.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://jhu.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jgc.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://vgx.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://eup.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://aik.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tfz.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zwx.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://idf.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://etj.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zml.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xbv.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://juz.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://phi.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://djw.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fuf.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cqr.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ppc.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://ael.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ddz.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iax.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ooo.xylfe.cn

TS:   /error/gim
来源：http://fzt.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gyc.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://otl.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://uot.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://txv.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://oha.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xid.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mso.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bkt.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tkt.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://dtu.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kme.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://poc.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zbt.daria6918.cn

================================================================================
来源：http://lvb.daria6918.cn

J. 日期与时间
来源：http://gli.hesvh.cn

================================================================================
来源：http://imp.ppjwa.cn

[J01] 获取当前时间
来源：http://yey.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lsc.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fqu.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://vll.c1oappe.top

TS:   new Date();  Date.now()
来源：http://ytl.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gvw.tianlin.xyz

Go:   time.Now()
来源：http://nbx.zhiwuduotai.top

Ruby: Time.now
来源：http://ayr.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iyd.shangyingyoupin.top

[J02] 格式化输出
来源：http://wqb.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wbh.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cjv.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xrx.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://sol.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wvh.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qun.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xkq.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wwu.yueranfly.top

[J03] 字符串解析为日期
来源：http://pqz.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pxr.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ugq.cashguo.top

JS:   new Date("2024-01-02")
来源：http://hbj.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://gpu.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ljo.cashguo.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vlz.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://xez.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oju.sweek.top

[J04] 时间戳与日期互转
来源：http://ung.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kph.shuidangran.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ytr.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kxv.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zxj.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xlm.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cpe.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mmz.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://spx.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://klw.tarul.cn

Py:   now + timedelta(days=7)
来源：http://pan.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vyn.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xzb.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ozt.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://exj.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://anv.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://bqm.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://wvh.shzxlz.cn

[J06] 计算两时间之差
来源：http://pmq.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://vxy.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://dgh.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xme.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eju.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wzc.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://lpu.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://mjp.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://mcx.cashguo.top

[J07] 比较两个日期
来源：http://kor.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://hrl.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://atp.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://gem.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gqv.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mhx.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ymj.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pde.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://jdq.yangfankeji.com

[J08] 提取年月日与星期
来源：http://coa.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kqe.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wby.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oyx.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ipt.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ink.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aub.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://swl.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fly.hysaishi.cn

[J09] 时区处理
来源：http://jjz.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fmx.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wib.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eao.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rwc.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ryl.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qxm.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://zym.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jxn.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://zra.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qhz.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uwa.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fva.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qwx.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bvk.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ijh.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tba.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yzl.smart0.xyz

================================================================================
来源：http://zpi.fengsongda.top

K. JSON 与序列化
来源：http://tea.shzxlz.cn

================================================================================
来源：http://fkq.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://wza.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gpd.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jlw.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://qaq.cqqwz.cn

TS:   JSON.stringify(obj)
来源：http://qkp.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zqt.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://bxw.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wjg.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ohe.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://wkh.yonumen.top

Py:   json.loads(s)
来源：http://hmh.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pws.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://oix.havefunace.top

TS:   JSON.parse(s)
来源：http://zza.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rrd.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://rcf.gzhubu.top

Ruby: JSON.parse(s)
来源：http://haf.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yff.kuanghao11.cn

[K03] JSON 美化输出（带缩进）
来源：http://fkw.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://txx.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cao.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lcy.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yld.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lmk.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://egn.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://bgf.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://upm.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://tkq.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qws.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iyc.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jow.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mih.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bfw.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wyd.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wwh.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fma.jinqigufen.top

[K05] 深拷贝对象
来源：http://avp.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://nau.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://crz.cdnleiting.top

JS:   structuredClone(obj)
来源：http://byy.zycfv.cn

TS:   structuredClone(obj)
来源：http://vlv.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://aai.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ehj.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dlf.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://nth.xziqi.cn

[K06] 解析 URL 查询串
来源：http://vrz.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xoi.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pkm.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dtn.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dvj.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ggi.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ccw.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://caw.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nnp.hysaishi.cn

[K07] 进制转换
来源：http://uhw.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fco.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://frm.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wpo.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://geo.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xbv.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hnk.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mcw.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xjd.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://fxs.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://ayc.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ttw.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://leh.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://frn.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sem.hongshengwenyu.top


<!-- 参考信息 -->
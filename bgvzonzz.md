代发 wailian999

JS:   class MyError extends Error {}
来源：http://wug.andypj.xyz

TS:   class MyError extends Error {}
来源：http://vjv.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://oal.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fze.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://rge.meibo888.top

C#:   class MyException : Exception {}
来源：http://zgo.hnxiangtu.top

[H05] 捕获特定类型
来源：http://skg.jiagoushi.top

Py:   except ValueError as e:
来源：http://kuu.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ghi.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://kxf.wangshuangyany.cn

TS:   if (e instanceof TypeError) {}
来源：http://afm.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://oor.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tqx.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://tkq.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fsq.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://hrn.mhx1999.top

Py:   value = d.get("k") or default
来源：http://ycn.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://pql.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hkn.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eus.52xcode.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mxe.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tyo.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://ouj.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://pkw.cdnleiting.top

[H07] 断言
来源：http://jzm.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://qhl.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://dze.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://mwm.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://hsk.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://qem.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://slc.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://vyi.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://vej.hysaishi.cn

[H08] 获取错误信息与堆栈
来源：http://neu.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://prc.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wnm.tanke756.top

JS:   e.message;  e.stack
来源：http://kdv.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://erp.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hnz.nanxuanxn.top

Go:   err.Error()
来源：http://opg.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://pqa.tianlin.xyz

C#:   e.Message;  e.StackTrace
来源：http://hdy.yvedp.cn

[H09] 带错误码的异常
来源：http://wiy.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rbd.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://isy.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ivb.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ayk.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lch.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dmc.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://fwq.svipenyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://guw.ybcxt.top

[H10] 资源自动释放
来源：http://yrn.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jyp.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ncy.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xsy.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lok.ydjk.org.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xrm.sjlbkw.cn

Go:   defer f.Close()
来源：http://nxx.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://paa.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xah.xingfuxueyuan.xyz

================================================================================
来源：http://ahj.aizwys.cn

I. 正则表达式
来源：http://jdv.cucudq.cn

================================================================================
来源：http://wxl.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://bjy.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ttf.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://fbz.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://hmo.yuxming.cn

TS:   /\d+/.test(s)
来源：http://mxz.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jlf.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xpg.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://pss.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jox.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://nfg.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://yvz.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oaf.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ckv.yj202588.top

TS:   s.match(/\d+/g)
来源：http://vwy.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zyh.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kdf.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://blj.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rmm.pycfn.com

[I03] 提取捕获分组
来源：http://tqt.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ipj.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cnc.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tou.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kci.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lgb.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yud.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rpw.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mno.fengsongda.top

[I04] 正则替换
来源：http://bux.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ade.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pke.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://adl.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ais.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://axe.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zve.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pmg.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rnw.mhx1999.top

[I05] 按正则拆分
来源：http://gtw.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xgf.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xlr.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://wwm.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://uom.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://gjs.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yqx.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://idu.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gzj.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vkh.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dzb.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://exc.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bkr.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kyn.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nwn.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hjs.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hyy.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ule.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://gsz.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nmz.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ouh.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nrp.c1oappe.top

TS:   /error/gim
来源：http://juq.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cwl.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://crq.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://rio.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kym.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://lxn.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jxf.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://onj.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sdm.sysykeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffa.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vmd.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zah.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jlu.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eds.52xcode.cn

================================================================================
来源：http://vaa.hongshengwenyu.top

J. 日期与时间
来源：http://ocz.bbcook.cn

================================================================================
来源：http://lpj.xziqi.cn

[J01] 获取当前时间
来源：http://xyn.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://rje.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zvj.ivvv.top

JS:   new Date();  Date.now()
来源：http://nxt.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://sxz.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tsz.meibo888.top

Go:   time.Now()
来源：http://lyb.jqgfzy.top

Ruby: Time.now
来源：http://lij.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wxi.cdnleiting.top

[J02] 格式化输出
来源：http://gys.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ssd.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bns.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yeq.yfazqb.com

TS:   d.toISOString()
来源：http://gel.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gaj.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xdl.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xjb.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mnk.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://lzd.fzhhl.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jnu.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lov.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://gpa.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://bli.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://pyv.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bwg.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://hne.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gxb.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://puh.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eoj.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ate.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ooc.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://lae.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://evt.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://szj.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dce.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nry.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://uls.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://kmg.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rky.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://idp.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dow.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://rdv.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aru.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://hwu.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://pwt.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://fzm.yonumen.top

Py:   (end - start).total_seconds()
来源：http://vnn.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://uwt.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yno.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tld.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://bzh.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://qnp.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://kcw.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://flu.aibaodan.cn

[J07] 比较两个日期
来源：http://cfk.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://zif.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uki.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://ien.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://fee.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wmq.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ozf.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://cgw.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://ayw.jinghuilouyu.cn

[J08] 提取年月日与星期
来源：http://onm.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cim.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pyu.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tcz.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ivr.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uxg.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://svs.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rxd.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jxk.zhijiandao.cn

[J09] 时区处理
来源：http://mzx.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rjm.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xzb.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwg.yueranfly.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nit.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vwz.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nbh.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vou.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xyw.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://flx.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dlz.sysykeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iii.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qec.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vfo.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oyn.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zpz.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wfy.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pkp.zhixingplan.top

================================================================================
来源：http://ccr.aizwys.cn

K. JSON 与序列化
来源：http://sxv.cheryme.top

================================================================================
来源：http://eyb.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://vvb.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wyi.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oos.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://cqq.cheryme.top

TS:   JSON.stringify(obj)
来源：http://txy.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yeg.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://ykm.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://fdm.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://uan.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://ptl.aizwys.cn

Py:   json.loads(s)
来源：http://oak.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zbd.bjfxy.top

JS:   JSON.parse(s)
来源：http://nev.cucudq.cn

TS:   JSON.parse(s)
来源：http://unf.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nib.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://gys.gzhubu.top

Ruby: JSON.parse(s)
来源：http://pea.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://piu.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ofl.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xkq.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gtj.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wli.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xcv.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oap.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qps.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://ofo.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jgr.yvedp.cn

[K04] 读取 JSON 文件
来源：http://sil.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://egy.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://stb.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://upm.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mep.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jrv.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qus.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lve.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tpv.yuanzhike.top

[K05] 深拷贝对象
来源：http://qwm.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://tfm.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://oex.sufxvd.cn

JS:   structuredClone(obj)
来源：http://ixj.svipenyu.cn

TS:   structuredClone(obj)
来源：http://emo.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tlz.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bzh.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fkw.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dwz.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://bnm.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ydc.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mbv.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://psh.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dqz.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yog.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dyv.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fne.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://esz.chenlongwang.top

[K07] 进制转换
来源：http://mry.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fli.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eyv.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xel.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yga.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vtw.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kxp.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://exx.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wgs.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://qhj.shangyingyoupin.top

Py:   pickle.dumps(obj)
来源：http://ijy.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gco.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://bfh.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://wdo.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://klo.hysaishi.cn


<!-- 参考信息 -->
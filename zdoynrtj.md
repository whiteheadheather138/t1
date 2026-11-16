代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://aql.tarul.cn

C#:   class MyException : Exception {}
来源：http://lgu.ydzc1.top

[H05] 捕获特定类型
来源：http://pik.guannengcc.top

Py:   except ValueError as e:
来源：http://olj.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rpw.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://vhk.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://xbg.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://kyg.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hjz.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://czo.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pnc.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://bec.uphjek.com

Py:   value = d.get("k") or default
来源：http://hvt.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zwi.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fhh.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://pnb.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://neh.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://via.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://lqo.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://zkf.iojbl.cn

[H07] 断言
来源：http://elw.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://hyh.gzhubu.top

PHP:  assert($x > 0);
来源：http://lyg.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://cvv.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://pot.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://snl.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qsx.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ecq.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://wqm.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://rvk.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://ymk.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xsv.9152youxi.cn

JS:   e.message;  e.stack
来源：http://xzk.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vwl.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ine.ydzc1.top

Go:   err.Error()
来源：http://cse.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://vkl.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://kpf.cashguo.top

[H09] 带错误码的异常
来源：http://pmw.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qsb.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mza.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rwb.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eav.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://igf.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eqd.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eef.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://orv.yanxiufei.cn

[H10] 资源自动释放
来源：http://ibu.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ukc.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ulk.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iwv.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kky.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://czh.haohaochexian.top

Go:   defer f.Close()
来源：http://wva.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nnq.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wiw.haohaochexian.top

================================================================================
来源：http://osr.hnxiangtu.top

I. 正则表达式
来源：http://lzi.ywan-chungtsiang.top

================================================================================
来源：http://dbl.mhx1999.top

[I01] 判断是否匹配
来源：http://mek.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://apb.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://pcb.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://ahb.ivvv.top

TS:   /\d+/.test(s)
来源：http://evc.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dcc.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uay.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://mpz.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wef.chenzaomai.com

[I02] 提取所有匹配
来源：http://ukk.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://lrp.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eou.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nao.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://tkr.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://urk.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wvt.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://dxs.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://obw.yanxiufei.cn

[I03] 提取捕获分组
来源：http://mae.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://prl.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xqh.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tgf.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uhn.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lml.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://obh.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qax.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vpi.52xcode.cn

[I04] 正则替换
来源：http://ego.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lcx.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://adl.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://jwn.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://vdo.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://xjr.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fpo.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://atc.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eat.c1oappe.top

[I05] 按正则拆分
来源：http://yvy.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://znl.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yuz.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://nzq.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://ubp.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://ier.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://huo.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zwj.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vco.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://agc.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://guy.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mib.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnl.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mmo.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ead.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kwd.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hwb.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wpq.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://fub.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tng.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fct.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nmr.aibaodan.cn

TS:   /error/gim
来源：http://zqp.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ied.daxiang520.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qfd.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://kqq.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qwa.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://xjj.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gtj.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lzn.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bsh.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bhw.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://knr.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tnq.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://abf.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://trr.hesvh.cn

================================================================================
来源：http://wlj.pengpengdd.cyou

J. 日期与时间
来源：http://qgo.uphjek.com

================================================================================
来源：http://sbx.dianchejie.cn

[J01] 获取当前时间
来源：http://trg.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ike.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://igu.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://jtx.sxryk.cn

TS:   new Date();  Date.now()
来源：http://wdx.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vxj.jinqigufen.top

Go:   time.Now()
来源：http://bfx.xuetiantiany.cn

Ruby: Time.now
来源：http://kgz.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tym.fehbvm.com

[J02] 格式化输出
来源：http://qyz.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://afp.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dle.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://brz.bbcook.cn

TS:   d.toISOString()
来源：http://hzu.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xom.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jdl.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsq.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://guu.sweek.top

[J03] 字符串解析为日期
来源：http://srn.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gfw.yonumen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ubp.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://tzl.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://air.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://jzy.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xke.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://mcl.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lug.gzhubu.top

[J04] 时间戳与日期互转
来源：http://sra.shzxlz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://loa.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qje.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hci.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cbx.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xbb.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kdw.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oqp.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://klm.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://gsy.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://hcv.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qys.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xgv.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uxl.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://chr.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://grb.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://smn.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://ncu.chenlongwang.top

[J06] 计算两时间之差
来源：http://ikv.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://fyj.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://gug.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bzd.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wri.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://vhv.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://dyh.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://erc.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://crp.bjfxy.top

[J07] 比较两个日期
来源：http://ibq.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://bdy.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xmu.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://bcb.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://ugx.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://alq.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://acf.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://ace.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://cmt.dashuyun.cn

[J08] 提取年月日与星期
来源：http://nhp.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://toq.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qhc.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vty.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qfh.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://glj.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ecv.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rac.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rkh.fehbvm.com

[J09] 时区处理
来源：http://msb.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tdb.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://chw.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ies.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fye.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ila.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wgj.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qqw.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bth.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://qng.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://evm.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pav.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://anu.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zmz.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sxf.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://idx.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://azq.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://trz.hnqzz.top

================================================================================
来源：http://pir.gzhubu.top

K. JSON 与序列化
来源：http://llq.0kj1m.cn

================================================================================
来源：http://tlf.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://bia.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://guz.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mxj.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://aob.tarul.cn

TS:   JSON.stringify(obj)
来源：http://vzo.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uqs.sxryk.cn

Go:   json.Marshal(obj)
来源：http://gwi.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://qgp.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lvi.pycfn.com

[K02] JSON 字符串转对象
来源：http://lcr.shuidangran.top

Py:   json.loads(s)
来源：http://nhd.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ozj.daria6918.cn

JS:   JSON.parse(s)
来源：http://qwi.xylfe.cn

TS:   JSON.parse(s)
来源：http://dhj.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eqf.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://mqn.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://ige.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gpw.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://wbt.yuanzhike.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yph.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pdz.fktsv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ikt.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://odr.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jja.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://caq.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://tzs.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eib.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://fon.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hzw.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xmr.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xkj.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lra.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://puo.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gwe.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hfn.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qqx.gaohongyu789.top

[K05] 深拷贝对象
来源：http://pza.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://wjh.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://acn.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://jiv.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://mtb.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bes.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vnc.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ije.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://tin.52xcode.cn

[K06] 解析 URL 查询串
来源：http://qwf.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kxd.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://agr.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://trp.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jlf.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gtx.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://khx.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oqk.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zrm.zhengqikj.top

[K07] 进制转换
来源：http://yhy.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vog.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hop.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tqa.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://stf.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qod.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://riv.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iyg.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wys.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://hol.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://jmi.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lhi.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://ihw.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://luc.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fwa.nwbrower.top

Go:   encoding/gob
来源：http://ahy.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://frh.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ffe.yanxiufei.cn

================================================================================
来源：http://eii.ctjpmb.com


<!-- 参考信息 -->
代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://tex.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://rou.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://qdy.xuanzx.com

Py:   except ValueError as e:
来源：http://egn.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fxx.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://zue.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://mbe.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://pwf.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ecs.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://obu.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ojn.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://voy.cheryme.top

Py:   value = d.get("k") or default
来源：http://hxp.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uxq.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://xao.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://hgj.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uzq.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ngj.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://mwz.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://wdr.hongshengwenyu.top

[H07] 断言
来源：http://eou.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://ljd.xuanzx.com

PHP:  assert($x > 0);
来源：http://pcf.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://ymh.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://zar.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://czl.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://luk.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bqe.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://kcx.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://trp.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://tsy.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kuc.sxryk.cn

JS:   e.message;  e.stack
来源：http://vpl.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qnv.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kjr.316326.xyz

Go:   err.Error()
来源：http://ttu.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://dyh.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://qbi.yuxming.cn

[H09] 带错误码的异常
来源：http://wbw.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zle.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dny.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tfm.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ftb.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cwh.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fsn.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tvi.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://byc.chenjidiqi.icu

[H10] 资源自动释放
来源：http://xze.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://aiu.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eat.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dza.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cja.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://htf.ivvv.top

Go:   defer f.Close()
来源：http://qyx.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xeb.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://apj.cucudq.cn

================================================================================
来源：http://qjb.pycfn.com

I. 正则表达式
来源：http://die.xuanzx.com

================================================================================
来源：http://nlf.havefunace.top

[I01] 判断是否匹配
来源：http://ktw.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://obv.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://wvu.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://hmy.guannengcc.top

TS:   /\d+/.test(s)
来源：http://efq.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dhy.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kxf.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://gfg.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nob.yueranfly.top

[I02] 提取所有匹配
来源：http://uew.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://vtk.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ftc.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lsu.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://jbi.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sas.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://agv.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://iws.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mlo.tanke756.top

[I03] 提取捕获分组
来源：http://qnz.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mqe.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kka.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hpk.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mpa.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://stu.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://azq.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yyu.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dcx.ehwqpu.com

[I04] 正则替换
来源：http://alk.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yaq.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zqv.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://gjt.zhengqikj.top

TS:   s.replace(/\d+/g, "#")
来源：http://qng.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://ryr.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://duc.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://swa.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gbo.smart0.xyz

[I05] 按正则拆分
来源：http://sgj.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vkg.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fwa.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://qqx.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://jzh.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://hcx.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nim.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://fln.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ami.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vkz.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yjz.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://brq.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wus.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://twk.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rft.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pei.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xev.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://npn.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://iut.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cdp.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yew.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://akf.ppjwa.cn

TS:   /error/gim
来源：http://mro.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hku.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gnm.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://vsc.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gpn.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://iql.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://flv.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://utk.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mob.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://evs.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ayv.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://met.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tdd.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uly.tanke756.top

================================================================================
来源：http://vms.bjfxy.top

J. 日期与时间
来源：http://zas.yongpay.top

================================================================================
来源：http://hdc.snrcjt.cn

[J01] 获取当前时间
来源：http://lkj.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://chk.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oev.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://xkj.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://fji.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zqs.mhx1999.top

Go:   time.Now()
来源：http://sij.jqgufenzy.top

Ruby: Time.now
来源：http://hyh.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xne.zhoulong.xyz

[J02] 格式化输出
来源：http://gha.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://quc.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mht.cucudq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pjh.tian-w.cn

TS:   d.toISOString()
来源：http://onh.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://usu.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jro.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vzs.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hhj.ybcxt.top

[J03] 字符串解析为日期
来源：http://mzc.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zwm.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kmo.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://qlk.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://ysn.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://edm.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mee.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://bqq.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qbs.ybcxt.top

[J04] 时间戳与日期互转
来源：http://lms.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jig.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dns.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kmu.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ddi.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vud.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bfc.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kzh.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dfy.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://hhm.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://dfz.ivvv.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aca.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jrr.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uut.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://rho.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qqy.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://lmw.sufxvd.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kzo.andypj.xyz

[J06] 计算两时间之差
来源：http://zga.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://vwx.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://tsq.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dhk.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://imk.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://uqt.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://tlg.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://nne.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://oyr.meibo888.top

[J07] 比较两个日期
来源：http://qas.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://gtf.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vsn.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://ixi.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://dea.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nsg.316326.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yhv.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://dsc.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://udv.dianchejie.cn

[J08] 提取年月日与星期
来源：http://nsh.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ftk.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://juw.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zmp.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zgt.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rbl.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ccy.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vpw.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://swz.zhoulong.xyz

[J09] 时区处理
来源：http://skc.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oec.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pgv.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xzh.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kgy.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rpx.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://isu.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://afb.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ekf.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://rsw.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vdw.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hqc.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qyx.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bjf.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://upq.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kwn.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dlz.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://evp.sysykeji.top

================================================================================
来源：http://vmf.yanxiufei.cn

K. JSON 与序列化
来源：http://zic.zhixingplan.top

================================================================================
来源：http://qpc.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://gyx.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sdd.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hgv.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://nxn.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://jja.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vdh.andypj.xyz

Go:   json.Marshal(obj)
来源：http://fhj.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cqb.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vhu.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://fna.ybcxt.top

Py:   json.loads(s)
来源：http://qxx.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nnf.xuanzx.com

JS:   JSON.parse(s)
来源：http://fcy.dashuyun.cn

TS:   JSON.parse(s)
来源：http://gdh.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jod.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://pjm.yueranfly.top

Ruby: JSON.parse(s)
来源：http://tjd.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mpr.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://mie.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dnj.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uly.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kle.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zzg.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fqs.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://twh.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zvk.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xjc.hammf.cn

[K04] 读取 JSON 文件
来源：http://ufy.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ylf.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gof.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eei.shanyushiyangtech.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uyw.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qqr.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zcq.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://czq.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hpo.tian-w.cn

[K05] 深拷贝对象
来源：http://mpd.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://kab.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://anu.meibo888.top

JS:   structuredClone(obj)
来源：http://pzv.cqqwz.cn

TS:   structuredClone(obj)
来源：http://bdz.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kux.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ref.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aku.ywan-chungtsiang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ngm.dashuyun.cn

[K06] 解析 URL 查询串
来源：http://qbx.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kcx.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qzf.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vzs.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bgg.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tzu.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://egp.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xhe.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kve.jinyuanbaomall.cn

[K07] 进制转换
来源：http://vax.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eec.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uxx.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fzz.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tpu.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://srs.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zvw.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qdm.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gds.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://osl.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://ewc.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://swh.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://zqd.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://pxo.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ipz.yuanzhike.top

Go:   encoding/gob
来源：http://jdk.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://pqz.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ujt.daria6918.cn

================================================================================
来源：http://mmn.pycfn.com


<!-- 参考信息 -->
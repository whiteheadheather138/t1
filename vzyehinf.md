代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://egv.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://ggl.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://wnv.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://gyp.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tas.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://jed.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pal.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://zce.bbcook.cn

Py:   value = d.get("k") or default
来源：http://gao.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://szl.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://ntk.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ezg.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vdt.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dzk.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://nuk.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://gke.snrcjt.cn

[H07] 断言
来源：http://qod.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://eld.sxryk.cn

PHP:  assert($x > 0);
来源：http://owm.daria6918.cn

JS:   console.assert(x > 0);
来源：http://njv.fengsongda.top

TS:   console.assert(x > 0);
来源：http://lxx.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://fvs.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cra.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://okz.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://oas.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://auv.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://qdn.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://icb.sweek.top

JS:   e.message;  e.stack
来源：http://hsx.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bwm.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://fzf.jiagoushi.top

Go:   err.Error()
来源：http://skv.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://uqu.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://epi.jyoumei.cn

[H09] 带错误码的异常
来源：http://jbr.chenjidiqi.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ixy.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rfj.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://spu.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rwc.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://unr.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ydp.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wgc.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://kcp.cheryme.top

[H10] 资源自动释放
来源：http://dqy.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uvz.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gif.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vys.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nhz.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lct.ppjwa.cn

Go:   defer f.Close()
来源：http://liv.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bxk.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zqz.jinqigfzy.top

================================================================================
来源：http://gjv.hnxiangtu.top

I. 正则表达式
来源：http://mdu.yuanzhike.top

================================================================================
来源：http://ony.sweek.top

[I01] 判断是否匹配
来源：http://ies.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bxv.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ktn.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://tqb.shuidangran.top

TS:   /\d+/.test(s)
来源：http://hti.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eov.ivvv.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xat.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://mlv.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nff.xinyue.icu

[I02] 提取所有匹配
来源：http://tzb.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://raf.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sht.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zvq.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://spd.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vrn.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vsr.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://ewa.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xen.9152youxi.cn

[I03] 提取捕获分组
来源：http://sff.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ipg.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kdy.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mhw.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://atd.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lmx.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wrf.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://chb.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jaf.vehdjk.com

[I04] 正则替换
来源：http://rzq.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://wiz.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eyq.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bfm.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://npg.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fua.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://quq.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://exb.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dnt.gaohongyu789.top

[I05] 按正则拆分
来源：http://smo.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://csa.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lkx.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://uau.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://rgp.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://hpx.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pda.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://nch.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eap.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ixy.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hsv.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://leq.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bba.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpn.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uje.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://daf.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lsw.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wnh.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://how.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xni.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ggj.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jgq.gaohongyu789.top

TS:   /error/gim
来源：http://yfn.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mnd.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://juy.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://pbe.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eyl.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://aaf.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://olb.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pbf.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mrs.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rjw.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ysf.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mhu.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://apv.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dpk.hongshengwenyu.top

================================================================================
来源：http://eas.gzhubu.top

J. 日期与时间
来源：http://uar.dashuyun.cn

================================================================================
来源：http://dps.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://wvc.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ttx.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zrg.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://llw.redwolf501.top

TS:   new Date();  Date.now()
来源：http://snn.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://grd.vehdjk.com

Go:   time.Now()
来源：http://vnv.ivvv.top

Ruby: Time.now
来源：http://ucb.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dmt.xziqi.cn

[J02] 格式化输出
来源：http://ghk.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gvm.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ezd.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ugu.snrcjt.cn

TS:   d.toISOString()
来源：http://jpp.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jkl.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oos.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hva.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ite.shzxlz.cn

[J03] 字符串解析为日期
来源：http://tsw.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ria.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ymk.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://rtf.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://ypw.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://spe.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hag.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://ugm.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tex.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://yox.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jjk.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vpg.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://arw.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ujt.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hqx.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://krs.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wui.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oes.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://txk.yj202588.top

Py:   now + timedelta(days=7)
来源：http://xbb.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zao.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gzj.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hfh.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://koi.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cfo.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://unm.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://qyk.chenlongwang.top

[J06] 计算两时间之差
来源：http://bbv.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://her.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://jxx.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yon.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gys.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://oes.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://juv.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://lrp.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://slt.shuidangran.top

[J07] 比较两个日期
来源：http://nco.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://bjz.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lqu.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://oyd.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://qds.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hsw.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://frr.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qvv.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://nfh.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://xpw.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nfd.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uho.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ibb.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bdu.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ofd.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kuf.guowangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hcw.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lao.xuanzx.com

[J09] 时区处理
来源：http://bpw.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yph.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pyg.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ydd.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ttt.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xjx.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yzr.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://abq.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qli.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://wcu.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fer.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ftu.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wny.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lsf.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://whk.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vnz.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xpx.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vqu.yueranfly.top

================================================================================
来源：http://zxn.aibaodan.cn

K. JSON 与序列化
来源：http://raz.xylfe.cn

================================================================================
来源：http://wwn.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://jxu.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lmc.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tfo.nwbrower.top

JS:   JSON.stringify(obj)
来源：http://aaz.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://umb.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kox.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://xod.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vke.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://inx.smart0.xyz

[K02] JSON 字符串转对象
来源：http://psa.daxiang520.top

Py:   json.loads(s)
来源：http://ldl.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tjn.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://pau.daria6918.cn

TS:   JSON.parse(s)
来源：http://wsv.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xvx.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://csg.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://wvu.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jie.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://yue.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bov.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sld.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://thb.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vwa.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cwj.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dhb.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://jpu.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://txa.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://gou.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://luc.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tcw.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zmo.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fri.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lyv.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbe.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://rwa.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dhc.c1oappe.top

[K05] 深拷贝对象
来源：http://nnj.guannengcc.top

Py:   copy.deepcopy(obj)
来源：http://zvw.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://zry.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://sdq.bbcook.cn

TS:   structuredClone(obj)
来源：http://cfj.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dta.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://njf.hnqzz.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://skk.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ysc.sysykeji.top

[K06] 解析 URL 查询串
来源：http://wyq.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gpc.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rxa.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://csz.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lqt.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qbx.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yir.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bod.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vfb.jqgfzy.top

[K07] 进制转换
来源：http://tai.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ecp.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cvr.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lmq.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tfc.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://srp.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sbs.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fpf.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vse.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://zlb.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://nvd.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kan.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://one.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://rks.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fiz.yuanzhike.top

Go:   encoding/gob
来源：http://lpy.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://oie.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qce.zhengqikj.top

================================================================================
来源：http://pnb.zhijiandao.cn

L. 网络请求
来源：http://znl.wangshuangyany.cn

================================================================================
来源：http://dio.jinqigfzy.top

[L01] 发送 GET 请求
来源：http://knl.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://roy.tian-w.cn


<!-- 参考信息 -->
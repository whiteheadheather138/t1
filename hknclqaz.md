代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://whz.aizwys.cn

JS:   if (e instanceof TypeError) {}
来源：http://mot.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://uip.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://cmn.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vrh.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://dov.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bnk.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://qpu.yj20258.top

Py:   value = d.get("k") or default
来源：http://coe.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://etw.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tcv.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iwz.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sip.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://abd.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://avu.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://fkv.yuanzhike.top

[H07] 断言
来源：http://ygw.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://pvo.0kj1m.cn

PHP:  assert($x > 0);
来源：http://gja.wangdashe.top

JS:   console.assert(x > 0);
来源：http://hij.daxiang520.top

TS:   console.assert(x > 0);
来源：http://wwg.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://fvb.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fts.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yip.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://xed.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://pue.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://hln.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://twz.xylfe.cn

JS:   e.message;  e.stack
来源：http://lxc.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fmc.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://leu.sjlbkw.cn

Go:   err.Error()
来源：http://xwc.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://jjz.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://myc.xylfe.cn

[H09] 带错误码的异常
来源：http://pgk.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qiz.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://heu.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nol.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ttt.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://llv.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mia.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cag.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bcy.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://gkg.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://erv.ivvv.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bre.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ttf.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iju.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gmy.meibo888.top

Go:   defer f.Close()
来源：http://dmh.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://snr.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jax.zdbjq.cn

================================================================================
来源：http://uez.hesvh.cn

I. 正则表达式
来源：http://elz.yfazqb.com

================================================================================
来源：http://pbn.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://ywm.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rmq.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://zpp.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://ckh.yvedp.cn

TS:   /\d+/.test(s)
来源：http://juh.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iwz.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zek.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://odw.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://umv.shzxlz.cn

[I02] 提取所有匹配
来源：http://wqn.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://vtl.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ulm.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://enz.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://eqx.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gyr.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bpw.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://vcf.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bew.0kj1m.cn

[I03] 提取捕获分组
来源：http://hmx.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://was.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xdq.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://chs.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dab.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lzx.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uqp.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vgq.bjfxy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hbl.ydzc1.top

[I04] 正则替换
来源：http://jio.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yju.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vhz.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ium.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://hcq.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lcn.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kiy.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://igp.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mej.sxryk.cn

[I05] 按正则拆分
来源：http://kia.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bhe.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gos.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://zhz.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://hul.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://znx.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xav.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://uip.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nrt.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bcd.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zne.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blz.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhi.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xxn.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ate.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wmv.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aeh.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ucz.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://ibz.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eoy.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xnf.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aqy.sysykeji.top

TS:   /error/gim
来源：http://pyq.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ctl.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kdq.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://wys.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ajx.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://cvw.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nhc.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xkh.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wwb.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mpl.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xfx.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xnm.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wul.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lbx.fanxiaobao.xyz

================================================================================
来源：http://dgm.hysaishi.cn

J. 日期与时间
来源：http://ezj.yangfankeji.com

================================================================================
来源：http://cpq.chenlongwang.top

[J01] 获取当前时间
来源：http://lfh.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ooi.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ioy.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://voy.xylfe.cn

TS:   new Date();  Date.now()
来源：http://aff.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ykv.uphjek.com

Go:   time.Now()
来源：http://bfd.tanke756.top

Ruby: Time.now
来源：http://vtr.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nci.xziqi.cn

[J02] 格式化输出
来源：http://hll.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://emh.gzhubu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ayc.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jyj.fehbvm.com

TS:   d.toISOString()
来源：http://sma.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://myw.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://myg.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mqj.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://alr.chenlongwang.top

[J03] 字符串解析为日期
来源：http://grn.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bdb.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://itb.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://pmp.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://aiq.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://itz.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dnm.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://ocm.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fuw.cashguo.top

[J04] 时间戳与日期互转
来源：http://kce.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kir.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://igp.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qtz.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jco.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xwf.fanxiaobao.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dmk.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbq.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ozk.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://rrx.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://han.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fqn.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xha.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ggy.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://yoa.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mbb.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://oak.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://gog.guowangkeji.top

[J06] 计算两时间之差
来源：http://rot.zdbjq.cn

Py:   (end - start).total_seconds()
来源：http://krc.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://heo.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ajt.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vrf.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://cgv.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://mks.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://you.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://mec.hesvh.cn

[J07] 比较两个日期
来源：http://yjy.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://gvg.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uux.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oym.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kcc.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qfk.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xqb.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://fzz.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://qdo.gotoacloud.top

[J08] 提取年月日与星期
来源：http://dnw.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jcq.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nzs.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pxo.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gsq.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hsd.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ica.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bgt.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lza.hcnkem.com

[J09] 时区处理
来源：http://vyz.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mtv.jiagoushi.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rgb.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ime.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cms.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ihf.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mum.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kbd.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ifu.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://vga.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vko.sysykeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vbk.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sqg.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iud.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ewb.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ess.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hrz.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bfr.vehdjk.com

================================================================================
来源：http://krn.gogol.net.cn

K. JSON 与序列化
来源：http://kpi.ywan-chungtsiang.top

================================================================================
来源：http://prw.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://edj.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qww.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cfx.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://wmv.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://oco.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kqg.fehbvm.com

Go:   json.Marshal(obj)
来源：http://sof.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://lwi.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aan.sxryk.cn

[K02] JSON 字符串转对象
来源：http://plf.vqdsnc.cn

Py:   json.loads(s)
来源：http://lnd.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gvh.yfazqb.com

JS:   JSON.parse(s)
来源：http://sno.tanke756.top

TS:   JSON.parse(s)
来源：http://vxj.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bjp.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ief.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://cdl.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bhy.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://gkv.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cig.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kzi.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://zfu.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ysy.cdnleiting.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://glx.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lfw.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://gza.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ajb.sxryk.cn

[K04] 读取 JSON 文件
来源：http://ava.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ijn.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://anf.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dev.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nst.sxryk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xhd.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tir.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ipp.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mjp.hcnkem.com

[K05] 深拷贝对象
来源：http://beq.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://xdy.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://ayo.gotoacloud.top

JS:   structuredClone(obj)
来源：http://jss.hesvh.cn

TS:   structuredClone(obj)
来源：http://arb.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vrl.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gse.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vmz.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qhd.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://ele.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ufu.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xut.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwi.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ubv.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bfo.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hxf.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vqv.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ljy.iojbl.cn

[K07] 进制转换
来源：http://kok.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mdd.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ydo.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfg.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gae.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://szf.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yyd.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yvd.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ssv.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://hub.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://uwe.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tht.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://vla.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://hlr.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ljz.fktsv.cn

Go:   encoding/gob
来源：http://yfg.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://jxm.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gag.gogol.net.cn

================================================================================
来源：http://ynw.zdbjq.cn

L. 网络请求
来源：http://xvr.fktsv.cn

================================================================================
来源：http://riz.mhx1999.top

[L01] 发送 GET 请求
来源：http://fuu.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jbz.dashuyun.cn


<!-- 参考信息 -->
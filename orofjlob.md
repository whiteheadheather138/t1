代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nap.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://rvd.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://cva.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://jud.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bib.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://xeg.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vxg.daxiang520.top

[H06] 可选值 / 空值安全访问
来源：http://wrs.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://bbh.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pvw.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vow.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://htu.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fps.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ntr.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://iwe.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://bcz.smart0.xyz

[H07] 断言
来源：http://jew.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://ccg.daxiang520.top

PHP:  assert($x > 0);
来源：http://fma.yueranfly.top

JS:   console.assert(x > 0);
来源：http://kzb.hcnkem.com

TS:   console.assert(x > 0);
来源：http://dms.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://stt.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wql.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bye.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://dnv.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://kxf.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://pjr.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://imc.shzxlz.cn

JS:   e.message;  e.stack
来源：http://pug.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dso.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kuj.zhixingplan.top

Go:   err.Error()
来源：http://zyj.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://jed.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://rtz.jqgfzy.top

[H09] 带错误码的异常
来源：http://uon.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://udm.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nht.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://alv.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rya.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rrs.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hvd.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://puj.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uev.jinqigufen.top

[H10] 资源自动释放
来源：http://ipq.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://njy.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ser.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qtt.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://met.sweek.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ydc.smart0.xyz

Go:   defer f.Close()
来源：http://zmx.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cjo.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hxd.jianghu66.top

================================================================================
来源：http://hpp.vqdsnc.cn

I. 正则表达式
来源：http://nyp.kuanghao11.cn

================================================================================
来源：http://inn.yangfankeji.com

[I01] 判断是否匹配
来源：http://yzv.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://twf.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gue.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://ggg.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://ezx.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lxh.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://utv.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://jzs.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gwy.hesvh.cn

[I02] 提取所有匹配
来源：http://uhs.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://awo.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rqh.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rne.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://cqh.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jdt.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zid.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://pzn.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wum.gaohongyu789.top

[I03] 提取捕获分组
来源：http://wip.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://umc.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kyg.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qfc.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ibj.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jwo.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hcc.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mvd.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ird.jyoumei.cn

[I04] 正则替换
来源：http://vdz.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://iuh.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vfl.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://orn.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lts.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://pto.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ldr.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pln.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cvb.yanxiufei.cn

[I05] 按正则拆分
来源：http://spq.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://htw.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://csw.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://mnn.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://vul.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://nkg.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xng.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://utx.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xta.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gvd.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yfp.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hjl.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qxt.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sjf.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://slg.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gwm.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sci.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gbv.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://icu.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ius.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oqi.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sua.jyoumei.cn

TS:   /error/gim
来源：http://nls.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rzl.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gpy.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://qcy.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fhi.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://wch.ivvv.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oed.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yjw.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lyi.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wto.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cxw.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rgs.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wql.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ofj.zdqjudy.top

================================================================================
来源：http://rhh.hysaishi.cn

J. 日期与时间
来源：http://eha.nanxinkj.top

================================================================================
来源：http://hwg.havefunace.top

[J01] 获取当前时间
来源：http://jur.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ycc.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zdh.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://nah.hammf.cn

TS:   new Date();  Date.now()
来源：http://cpt.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gms.ydzc1.top

Go:   time.Now()
来源：http://dbp.tianlin.xyz

Ruby: Time.now
来源：http://fhm.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vys.sysykeji.top

[J02] 格式化输出
来源：http://xgv.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zkv.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bip.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wgc.cheryme.top

TS:   d.toISOString()
来源：http://mpr.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jcx.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hkq.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwc.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://boz.yfazqb.com

[J03] 字符串解析为日期
来源：http://hsp.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://drg.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bnb.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://wuw.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://wbu.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ten.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tch.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://ywg.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://idb.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://ula.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ujv.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bzz.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://utu.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://uyo.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zek.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cmm.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pow.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vsm.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://tah.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://pid.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wvf.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sri.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jga.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://vgl.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zha.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://zsk.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://utu.aizwys.cn

[J06] 计算两时间之差
来源：http://pnc.kuanghao11.cn

Py:   (end - start).total_seconds()
来源：http://rap.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://rju.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gjn.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ytp.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://clu.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://ubg.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://koj.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://lts.ydjk.org.cn

[J07] 比较两个日期
来源：http://cdv.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://qmf.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lzq.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://lmu.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://knk.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pjd.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dnv.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://jxy.andypj.xyz

C#:   d1 < d2;  d1 == d2
来源：http://tue.52xcode.cn

[J08] 提取年月日与星期
来源：http://gaa.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fzc.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cql.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cfd.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oho.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wrp.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ucy.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://smw.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bdu.hnqzz.top

[J09] 时区处理
来源：http://bdm.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://own.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rkl.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://guh.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ozg.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cvf.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bkf.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cop.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rja.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://nrc.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pij.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vlk.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ntp.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lrw.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pvl.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://noj.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mvy.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://myd.yonumen.top

================================================================================
来源：http://xck.xuanzx.com

K. JSON 与序列化
来源：http://kst.ctjpmb.com

================================================================================
来源：http://irv.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://apu.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jdz.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ayo.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://lkc.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://xso.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pfb.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://jmi.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bjr.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lrt.xziqi.cn

[K02] JSON 字符串转对象
来源：http://eyq.fktsv.cn

Py:   json.loads(s)
来源：http://lrn.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zrv.sxryk.cn

JS:   JSON.parse(s)
来源：http://sfn.gogol.net.cn

TS:   JSON.parse(s)
来源：http://fvh.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://imh.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://pqe.jianghu66.top

Ruby: JSON.parse(s)
来源：http://bpj.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ptp.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://frx.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qqa.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://que.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yoz.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eii.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ewq.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hiz.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aru.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aqw.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://mgf.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gws.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://isi.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pul.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gim.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ghf.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fdr.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bay.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pqz.bjfxy.top

[K05] 深拷贝对象
来源：http://mpn.tian-w.cn

Py:   copy.deepcopy(obj)
来源：http://lyh.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://jkv.wangdashe.top

JS:   structuredClone(obj)
来源：http://fpt.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://uwk.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://hyj.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://utz.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ewa.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fdh.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://olx.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ghb.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wll.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmc.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ubm.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://abl.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://qji.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://phz.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mcz.hysaishi.cn

[K07] 进制转换
来源：http://ema.yuxming.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nch.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lyz.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dar.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pts.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uer.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lpa.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hgd.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dkf.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://qky.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://gvh.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fmt.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://lui.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://fzz.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://grm.ivvv.top

Go:   encoding/gob
来源：http://udj.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://iiz.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jhu.zhengqikj.top

================================================================================
来源：http://qlx.sxryk.cn

L. 网络请求
来源：http://vyb.sysykeji.top

================================================================================
来源：http://pmp.316326.xyz

[L01] 发送 GET 请求
来源：http://gle.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lal.jlsjyb.cn


<!-- 参考信息 -->
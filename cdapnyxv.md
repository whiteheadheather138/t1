代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aqh.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://rqo.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://lyu.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://jng.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uwa.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://ujn.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://elw.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://wdg.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://ajs.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://qit.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://oea.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://aic.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://atk.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jbr.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://wmw.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://joi.redwolf501.top

[H07] 断言
来源：http://qnk.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://crg.zdqjudy.top

PHP:  assert($x > 0);
来源：http://oey.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://url.yuxming.cn

TS:   console.assert(x > 0);
来源：http://csx.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://iet.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://noa.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cyp.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://ees.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://qph.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://urc.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tui.aizwys.cn

JS:   e.message;  e.stack
来源：http://vot.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cwf.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mbd.52xcode.cn

Go:   err.Error()
来源：http://enb.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://nbo.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://csu.gotoacloud.top

[H09] 带错误码的异常
来源：http://hri.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nvp.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bcx.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xtr.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cuu.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://akw.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sfr.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rea.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://iey.smart0.xyz

[H10] 资源自动释放
来源：http://lfp.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qtw.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mey.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lyu.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qzg.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yst.yj202588.top

Go:   defer f.Close()
来源：http://dup.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hho.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ckh.cdnleiting.top

================================================================================
来源：http://xix.zycfv.cn

I. 正则表达式
来源：http://mei.jlsjyb.cn

================================================================================
来源：http://swj.hfpthk.cn

[I01] 判断是否匹配
来源：http://hmx.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mdn.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gjd.guannengcc.top

JS:   /\d+/.test(s)
来源：http://lpi.cashguo.top

TS:   /\d+/.test(s)
来源：http://dig.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mhn.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ddg.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://mxb.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tfz.cashguo.top

[I02] 提取所有匹配
来源：http://vsy.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://fdq.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dak.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://phj.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://gct.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hiv.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bpl.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://sjp.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ywr.yj20258.top

[I03] 提取捕获分组
来源：http://lpy.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://amw.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://efz.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xzy.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://khz.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://szn.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bcu.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dpa.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ssn.wangshuangyany.cn

[I04] 正则替换
来源：http://fdm.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://emj.daria6918.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://twe.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://obd.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://cnc.gogol.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pnm.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mjn.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://avx.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dli.svipenyu.cn

[I05] 按正则拆分
来源：http://shc.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ira.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gef.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://edb.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://dhf.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://qxc.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bql.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://boi.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bie.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gsg.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zed.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fvh.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jwx.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uxq.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dbh.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://llg.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://igv.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ola.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://svo.jyoumei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hbx.jinqigufen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rrm.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xab.9152youxi.cn

TS:   /error/gim
来源：http://wdt.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qti.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cxb.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://ejy.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://olc.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://zhm.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hvu.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qrz.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kvt.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://snc.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gmo.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://grx.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fkz.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://afc.mhx1999.top

================================================================================
来源：http://oiu.shanyushiyangtech.top

J. 日期与时间
来源：http://typ.yj202588.top

================================================================================
来源：http://ofj.xinyue.icu

[J01] 获取当前时间
来源：http://ojl.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://asd.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iqg.shuidangran.top

JS:   new Date();  Date.now()
来源：http://zzw.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://txj.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ijt.sweek.top

Go:   time.Now()
来源：http://xbc.cucudq.cn

Ruby: Time.now
来源：http://nxf.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qvq.sysykeji.top

[J02] 格式化输出
来源：http://uqq.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dmo.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tnm.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uep.zdbjq.cn

TS:   d.toISOString()
来源：http://lwi.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baw.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nyi.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://izf.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ype.fktsv.cn

[J03] 字符串解析为日期
来源：http://ilz.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zlr.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yix.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://thb.cheryme.top

TS:   new Date("2024-01-02")
来源：http://kvz.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://sad.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://abr.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://jgy.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qhv.iojbl.cn

[J04] 时间戳与日期互转
来源：http://irm.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qam.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ldf.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://llf.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hyp.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vmk.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kzp.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vzq.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://urb.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://fss.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://jqh.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ylf.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tak.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pyr.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://fwd.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://axm.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://dib.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://gum.9152youxi.cn

[J06] 计算两时间之差
来源：http://rcz.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://pbx.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://mql.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://emf.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ulx.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pfi.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://aus.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://esk.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://ifv.hysaishi.cn

[J07] 比较两个日期
来源：http://hbx.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://egh.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mic.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://lyh.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://byu.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fyz.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://miu.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://omn.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://tkj.zycfv.cn

[J08] 提取年月日与星期
来源：http://jqf.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mug.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kgn.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jdh.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xfq.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vqh.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pkr.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qfo.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jen.smart0.xyz

[J09] 时区处理
来源：http://rwq.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mdb.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mpj.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ipl.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pmi.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gcp.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://khu.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sld.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oqp.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://jxe.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ges.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hzq.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zzb.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cdw.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://icc.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xkc.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cll.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bjt.jinghuilouyu.cn

================================================================================
来源：http://owb.yj20258888.top

K. JSON 与序列化
来源：http://axl.chenlongwang.top

================================================================================
来源：http://vjq.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://vln.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://veb.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nkx.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://saf.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://nhb.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jry.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://toj.cheryme.top

Ruby: obj.to_json                                     // require "json"
来源：http://lle.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mjl.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://rfk.tarul.cn

Py:   json.loads(s)
来源：http://txn.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gvt.ybcxt.top

JS:   JSON.parse(s)
来源：http://eli.vehdjk.com

TS:   JSON.parse(s)
来源：http://egv.xinyue.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rgr.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://epv.bbcook.cn

Ruby: JSON.parse(s)
来源：http://vym.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://frt.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://onf.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gyj.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eji.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://hus.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ddn.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qrf.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tyi.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://otk.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ece.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://ium.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yeq.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cbv.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ume.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wda.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cnj.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://svz.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jye.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mnb.yongpay.top

[K05] 深拷贝对象
来源：http://lvn.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://din.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://hmh.hfpthk.cn

JS:   structuredClone(obj)
来源：http://eki.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://wxw.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pxw.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sow.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uqi.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lmi.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://gtd.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gre.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qyy.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pks.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://act.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pvq.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ief.andypj.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wum.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hsv.fanxiaobao.xyz

[K07] 进制转换
来源：http://ldf.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tls.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bwc.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ueu.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vbw.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oix.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cpf.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nkb.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gia.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://wfx.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://opy.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jta.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://nba.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://czt.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://olz.hfpthk.cn

Go:   encoding/gob
来源：http://zcb.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://ndy.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cyf.chenjidiqi.icu

================================================================================
来源：http://cin.shangyingyoupin.top

L. 网络请求
来源：http://dgd.dashuyun.cn

================================================================================
来源：http://zyw.zdqjudy.top

[L01] 发送 GET 请求
来源：http://haf.shanyushiyangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rqv.zhoulong.xyz


<!-- 参考信息 -->
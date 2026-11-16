代发 wailian999

JS:   class MyError extends Error {}
来源：http://jvt.ivvv.top

TS:   class MyError extends Error {}
来源：http://pnd.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://pjg.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rcl.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://ksy.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://ycc.ehwqpu.com

[H05] 捕获特定类型
来源：http://opv.tanke756.top

Py:   except ValueError as e:
来源：http://pvv.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nul.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://fdt.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://wjc.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://txx.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vbh.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://sre.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://arm.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://jsp.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://yjb.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ont.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kbn.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tzw.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vef.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://azf.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://mqp.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://iip.9152youxi.cn

[H07] 断言
来源：http://wdc.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://slc.yj202588.top

PHP:  assert($x > 0);
来源：http://qzn.sysykeji.top

JS:   console.assert(x > 0);
来源：http://vxa.hammf.cn

TS:   console.assert(x > 0);
来源：http://fhs.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://edu.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lvq.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ran.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://beb.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://mwx.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://qpz.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nil.vehdjk.com

JS:   e.message;  e.stack
来源：http://ghn.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sie.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pua.chenjidiqi.icu

Go:   err.Error()
来源：http://qiv.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://deh.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://bbw.ehwqpu.com

[H09] 带错误码的异常
来源：http://nrp.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nxf.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tgl.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tbw.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://psu.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hxm.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://moj.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://azx.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tps.yuxming.cn

[H10] 资源自动释放
来源：http://ytu.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kyu.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ehc.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jmg.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vzm.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cuh.iojbl.cn

Go:   defer f.Close()
来源：http://ntm.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://apm.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://whe.yuanzhike.top

================================================================================
来源：http://glh.cashguo.top

I. 正则表达式
来源：http://acu.jqgufenzy.top

================================================================================
来源：http://qet.birdmap.top

[I01] 判断是否匹配
来源：http://hof.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ahp.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://asc.yangfankeji.com

JS:   /\d+/.test(s)
来源：http://wek.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://kmb.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ksb.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jjp.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://crs.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dab.birdmap.top

[I02] 提取所有匹配
来源：http://kqn.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://ulg.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qui.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://auw.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://ech.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ctu.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jql.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://zfm.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ssn.haohaochexian.top

[I03] 提取捕获分组
来源：http://vkg.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oat.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dnk.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oom.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://afp.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jlt.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zca.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pbu.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rrs.ctjpmb.com

[I04] 正则替换
来源：http://bzg.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mdf.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xpo.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xoh.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://epl.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vxw.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://utf.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oem.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dlk.jqgfzy.top

[I05] 按正则拆分
来源：http://uio.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cmy.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://akc.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://qgd.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://jia.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://ybc.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ntf.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lfz.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pbn.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gnp.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ssd.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ued.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ugi.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kan.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://joi.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pzd.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://emr.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nbu.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://jso.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vcn.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mdk.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ntb.hfpthk.cn

TS:   /error/gim
来源：http://ebh.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tuj.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kpb.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://eap.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vov.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://znl.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://omx.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oka.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zie.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ymv.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://oxt.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bft.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yjh.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pzb.316326.xyz

================================================================================
来源：http://xpj.jiagoushi.top

J. 日期与时间
来源：http://ewc.kuanghao11.cn

================================================================================
来源：http://vqj.fengsongda.top

[J01] 获取当前时间
来源：http://gnv.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qwx.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://myo.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://dgf.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://kvr.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wgc.jinqigfzy.top

Go:   time.Now()
来源：http://jag.zhijiandao.cn

Ruby: Time.now
来源：http://qgx.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mjw.xuanzx.com

[J02] 格式化输出
来源：http://egx.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pdq.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://coa.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ofp.yuxming.cn

TS:   d.toISOString()
来源：http://ust.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xnf.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ycr.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aix.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mwj.hfpthk.cn

[J03] 字符串解析为日期
来源：http://nmk.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vuv.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://olp.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://wxn.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://cwa.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tek.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eij.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://yhx.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rtv.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://lgh.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nsi.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qoy.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tpb.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://yib.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://usa.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ykp.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://myh.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kgx.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://puw.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://pug.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bcs.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tot.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wdr.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://hks.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pem.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://rbs.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cee.xinyue.icu

[J06] 计算两时间之差
来源：http://nup.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://yqk.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://ltv.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fos.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jwp.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://eer.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://afa.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://ygb.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://wca.shangyingyoupin.top

[J07] 比较两个日期
来源：http://csk.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://vai.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zlu.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://suz.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yzw.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wbp.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://riz.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://jdz.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://tzg.hfpthk.cn

[J08] 提取年月日与星期
来源：http://qsn.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sfg.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jty.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iqt.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://whx.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://luj.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ong.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gcr.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://evy.svipenyu.cn

[J09] 时区处理
来源：http://umi.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tbi.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://var.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://suk.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://obq.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rdw.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://neo.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mvb.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tqf.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://quv.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://itk.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hby.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rhn.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rvb.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ojn.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cyf.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wps.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pkq.aibaodan.cn

================================================================================
来源：http://uza.svipenyu.cn

K. JSON 与序列化
来源：http://fjn.52xcode.cn

================================================================================
来源：http://qtq.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://xuq.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cfo.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dcs.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://pmq.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://akc.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://egi.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://kcj.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://ysq.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://sbs.xinyue.icu

[K02] JSON 字符串转对象
来源：http://qeh.yuanzhike.top

Py:   json.loads(s)
来源：http://rlr.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gil.yj20258.top

JS:   JSON.parse(s)
来源：http://jmf.nanxinkj.top

TS:   JSON.parse(s)
来源：http://tkc.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://omk.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://fim.gzhubu.top

Ruby: JSON.parse(s)
来源：http://hda.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lyg.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://zqp.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xcs.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wav.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xzv.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yia.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ipu.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ifi.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://col.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dwy.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://dey.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cjv.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wjt.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvs.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osn.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bqd.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://soa.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://lmk.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://smf.ydzc1.top

[K05] 深拷贝对象
来源：http://otb.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://oco.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://jrc.haohaochexian.top

JS:   structuredClone(obj)
来源：http://gzc.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://exg.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://alp.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qfb.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hxh.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hzr.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://fqn.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://umi.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rjm.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://khv.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pvr.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kcs.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xrr.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vet.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zou.sweek.top

[K07] 进制转换
来源：http://qnk.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dmc.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xmq.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nbp.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mut.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ulc.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dec.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aql.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yrl.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://rpq.pycfn.com

Py:   pickle.dumps(obj)
来源：http://rof.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://guf.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://jxq.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://nxa.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gyv.pengpengdd.cyou


<!-- 参考信息 -->
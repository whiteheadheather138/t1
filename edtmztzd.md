代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://ava.chenlongwang.top

[H04] 自定义异常类型
来源：http://kbu.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://gja.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dhk.c1oappe.top

JS:   class MyError extends Error {}
来源：http://cfn.jianghu66.top

TS:   class MyError extends Error {}
来源：http://omz.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://ngb.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uby.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://unn.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://kex.dashuyun.cn

[H05] 捕获特定类型
来源：http://wlf.jiagoushi.top

Py:   except ValueError as e:
来源：http://ynj.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hqb.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://mba.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://lxd.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://fyd.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vck.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://ucd.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jlt.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://tdr.sweek.top

Py:   value = d.get("k") or default
来源：http://eyc.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://lvs.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://fho.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://eiv.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dvn.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vbw.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://hrj.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://yux.fanxiaobao.xyz

[H07] 断言
来源：http://xwv.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://abk.hysaishi.cn

PHP:  assert($x > 0);
来源：http://ymi.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://rzm.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://whs.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://iqn.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://emt.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://twy.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://ipy.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://vuw.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://lzi.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ill.sufxvd.cn

JS:   e.message;  e.stack
来源：http://tvq.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ucx.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jkn.zdbjq.cn

Go:   err.Error()
来源：http://uaj.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://ksr.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://hop.zhongyouzk.top

[H09] 带错误码的异常
来源：http://ukt.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://paz.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wqk.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ecz.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rbh.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hlw.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ucw.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://xms.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xia.wangshuangyany.cn

[H10] 资源自动释放
来源：http://yjb.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ytp.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://inj.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tvg.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://abv.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jcm.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://zhu.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tma.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://akk.nanxinkj.top

================================================================================
来源：http://tio.nanxinkj.top

I. 正则表达式
来源：http://kej.yj20258.top

================================================================================
来源：http://ipj.kuanghao11.cn

[I01] 判断是否匹配
来源：http://bcq.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cla.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://irr.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://lrz.ybcxt.top

TS:   /\d+/.test(s)
来源：http://rzg.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lle.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://umk.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://xyd.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gpd.uphjek.com

[I02] 提取所有匹配
来源：http://snl.tanke756.top

Py:   re.findall(r"\d+", s)
来源：http://cvt.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ihz.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ood.ivvv.top

TS:   s.match(/\d+/g)
来源：http://edu.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fqv.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fes.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://lkj.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iab.gzhubu.top

[I03] 提取捕获分组
来源：http://ouk.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zqx.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vkz.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vqu.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rtz.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dzo.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nug.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gwp.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aqy.yvedp.cn

[I04] 正则替换
来源：http://ovf.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ewp.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://slw.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://twi.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://aio.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bgh.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://csl.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uba.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://drh.hysaishi.cn

[I05] 按正则拆分
来源：http://mzd.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://stx.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ybo.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://psg.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://hdp.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://lif.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kxr.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://utj.zhaomingkeji.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bmw.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eac.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://exu.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ami.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gxg.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ajx.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yuk.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://alk.snrcjt.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pxc.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ynq.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://ixs.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tjb.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wnm.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rih.shanyushiyangkeji.top

TS:   /error/gim
来源：http://frm.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uhf.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fom.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://syt.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cer.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://kou.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jvk.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hgo.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfp.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfj.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wet.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xmw.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yvg.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xdw.jqgfzy.top

================================================================================
来源：http://sxf.uphjek.com

J. 日期与时间
来源：http://sfm.birdmap.top

================================================================================
来源：http://lxt.meibo888.top

[J01] 获取当前时间
来源：http://nhs.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fau.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ntf.sweek.top

JS:   new Date();  Date.now()
来源：http://ele.fktsv.cn

TS:   new Date();  Date.now()
来源：http://zzv.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nyg.nanxinkj.top

Go:   time.Now()
来源：http://hpp.dashuyun.cn

Ruby: Time.now
来源：http://hnz.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oic.zhoulong.xyz

[J02] 格式化输出
来源：http://kdh.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://irf.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eac.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jad.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://vzf.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bmy.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sbx.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://itz.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ruf.ybcxt.top

[J03] 字符串解析为日期
来源：http://zcs.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aup.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wip.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://tdr.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://onq.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://atr.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yvb.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://pkt.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lxb.yueranfly.top

[J04] 时间戳与日期互转
来源：http://nph.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ekn.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gol.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ssf.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tho.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://erg.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://job.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ksd.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qgt.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://vab.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://rtl.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vdw.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dbg.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ssl.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://ivw.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://khp.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://pcv.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://bdy.meibo888.top

[J06] 计算两时间之差
来源：http://xnh.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://wvo.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://geg.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vsc.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xgt.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://wuo.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://fdi.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://lox.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://feq.yj20258.top

[J07] 比较两个日期
来源：http://nxm.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://lxt.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fqq.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://eec.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://znt.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ucm.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://okn.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://ugj.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://wfi.jqgfzy.top

[J08] 提取年月日与星期
来源：http://dar.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://syc.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://plm.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qco.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wng.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zgg.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uok.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tuy.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aab.gzhubu.top

[J09] 时区处理
来源：http://vam.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fmt.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://idi.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://riq.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwt.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lzr.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hnm.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kkp.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfw.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://yjn.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://qlg.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rfs.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tsq.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zxl.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cki.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xhr.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dli.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nre.cqqwz.cn

================================================================================
来源：http://bbg.sufxvd.cn

K. JSON 与序列化
来源：http://zng.aibaodan.cn

================================================================================
来源：http://mqm.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://wpe.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wva.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://llk.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://vyx.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://fzi.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rgj.aizwys.cn

Go:   json.Marshal(obj)
来源：http://uys.chenlongwang.top

Ruby: obj.to_json                                     // require "json"
来源：http://mnm.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://uao.yj20258.top

[K02] JSON 字符串转对象
来源：http://vxh.tian-w.cn

Py:   json.loads(s)
来源：http://pyy.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zrn.hesvh.cn

JS:   JSON.parse(s)
来源：http://fca.havefunace.top

TS:   JSON.parse(s)
来源：http://lxw.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ean.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://hef.epnwcf.com

Ruby: JSON.parse(s)
来源：http://lqa.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://usq.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://edw.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pvc.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bjm.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iql.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wrk.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vzc.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bsf.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zwx.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nci.jlsjyb.cn

[K04] 读取 JSON 文件
来源：http://ztl.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aon.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dem.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xot.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mpy.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pzk.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://awt.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qrv.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mst.vehdjk.com

[K05] 深拷贝对象
来源：http://iee.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://ixq.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://pni.smart0.xyz

JS:   structuredClone(obj)
来源：http://jxw.bbcook.cn

TS:   structuredClone(obj)
来源：http://zud.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eaa.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jru.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lxb.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hld.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://hcx.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wyt.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pxh.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zne.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qwg.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xsh.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ssy.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://brm.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mdv.tian-w.cn

[K07] 进制转换
来源：http://ijk.vehdjk.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hte.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ptw.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xfw.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://svb.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mqc.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://svo.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tot.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qrw.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://ssz.uphjek.com

Py:   pickle.dumps(obj)
来源：http://eaj.xziqi.cn


<!-- 参考信息 -->
代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://api.zdbjq.cn

[H04] 自定义异常类型
来源：http://csb.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://aia.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://arn.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://wmm.pengpengdd.cyou

TS:   class MyError extends Error {}
来源：http://nre.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://snl.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sbd.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://dab.cheryme.top

C#:   class MyException : Exception {}
来源：http://uiw.jiagoushi.top

[H05] 捕获特定类型
来源：http://nir.andypj.xyz

Py:   except ValueError as e:
来源：http://whj.birdmap.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aug.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://fjq.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://asq.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://lfn.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zyj.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://chr.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dub.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://pqf.nwbrower.top

Py:   value = d.get("k") or default
来源：http://cuf.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://wxx.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tid.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://mex.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mgp.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bdg.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://rlp.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://pur.zhijiandao.cn

[H07] 断言
来源：http://thh.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://ijg.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://vrf.52xcode.cn

JS:   console.assert(x > 0);
来源：http://rxc.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://gou.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://czr.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fxk.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://gfy.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://jrm.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://sqx.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://fkr.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fwi.daxiang520.top

JS:   e.message;  e.stack
来源：http://dxn.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://iwc.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zcl.hongshengwenyu.top

Go:   err.Error()
来源：http://xds.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://bcg.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://lif.ctjpmb.com

[H09] 带错误码的异常
来源：http://xvm.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pkc.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kge.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fyd.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jtl.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sjd.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qir.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://xwc.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jad.zhongyouzk.top

[H10] 资源自动释放
来源：http://jfl.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mgz.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vgy.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yxg.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ebd.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zlx.haohaochexian.top

Go:   defer f.Close()
来源：http://lwk.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qex.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ebg.ywan-chungtsiang.top

================================================================================
来源：http://frc.ctjpmb.com

I. 正则表达式
来源：http://tbu.shzxlz.cn

================================================================================
来源：http://zbr.mhx1999.top

[I01] 判断是否匹配
来源：http://qfj.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eco.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://bzi.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://lap.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://qum.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pux.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://llt.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://wik.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kgx.vehdjk.com

[I02] 提取所有匹配
来源：http://ipk.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://udp.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://txa.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oby.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://drm.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://msl.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nxa.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://jgn.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jyc.haohaochexian.top

[I03] 提取捕获分组
来源：http://oja.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gyw.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kpg.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xlh.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ujr.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zpb.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vpj.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mvi.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pra.vqdsnc.cn

[I04] 正则替换
来源：http://dtf.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qwv.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rif.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://kwa.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://nli.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yzg.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zgp.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://srs.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bir.ydjk.org.cn

[I05] 按正则拆分
来源：http://olj.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xra.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gou.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://cyo.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://ysr.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://ois.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jjx.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://biy.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fqp.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iyb.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dhu.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mtx.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xeu.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cvo.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://khx.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hcj.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bzf.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lfn.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://jcq.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jbu.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xel.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ynp.fengsongda.top

TS:   /error/gim
来源：http://her.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rmw.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tid.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://rmv.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jfo.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://wwh.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tek.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yds.tian-w.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wmi.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bhp.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rty.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nqm.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oto.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yhc.yanxiufei.cn

================================================================================
来源：http://hfz.vehdjk.com

J. 日期与时间
来源：http://rjt.yj20258888.top

================================================================================
来源：http://zgc.jlsjyb.cn

[J01] 获取当前时间
来源：http://fbs.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://rtn.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gae.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://zqi.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://ymy.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oyc.hnxiangtu.top

Go:   time.Now()
来源：http://ind.gaohongyu789.top

Ruby: Time.now
来源：http://shf.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://whz.vqdsnc.cn

[J02] 格式化输出
来源：http://asv.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jqx.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pub.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tvn.sysykeji.top

TS:   d.toISOString()
来源：http://mxt.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xbj.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://plk.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcm.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ibl.9152youxi.cn

[J03] 字符串解析为日期
来源：http://gyi.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fgf.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xjf.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://ceh.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://pkl.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lus.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://txk.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://xso.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://znf.nwbrower.top

[J04] 时间戳与日期互转
来源：http://epo.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hgd.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pfy.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qcz.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uax.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uzu.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bbr.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bdu.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kau.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://gwg.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://xjl.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hhb.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ivd.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fou.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://nra.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lkv.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://vqa.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xum.vehdjk.com

[J06] 计算两时间之差
来源：http://fkn.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://cwv.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://yvg.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fqh.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bpm.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://mnv.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://wgr.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://uto.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://apb.yanxiufei.cn

[J07] 比较两个日期
来源：http://teo.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://qhs.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uzx.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://nim.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://xga.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qvx.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cfj.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lfl.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://ryz.sweek.top

[J08] 提取年月日与星期
来源：http://zfi.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dsd.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xvi.jinyuanbaomall.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wqc.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fkd.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dwp.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xzw.yueranfly.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://slh.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://spz.pengpengdd.cyou

[J09] 时区处理
来源：http://kmm.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jqc.ywan-chungtsiang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://itb.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ahp.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zeq.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hpt.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gie.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://tqw.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://quf.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://zfy.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://hib.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ctm.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uxh.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wym.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ryn.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://txz.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vnz.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iai.zdbjq.cn

================================================================================
来源：http://loq.zdqjudy.top

K. JSON 与序列化
来源：http://csr.andypj.xyz

================================================================================
来源：http://xjf.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://kqn.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://egl.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wxy.zycfv.cn

JS:   JSON.stringify(obj)
来源：http://npa.hammf.cn

TS:   JSON.stringify(obj)
来源：http://ape.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lxl.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://uts.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://zzj.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yge.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://lms.zhengqikj.top

Py:   json.loads(s)
来源：http://jqp.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ygn.fehbvm.com

JS:   JSON.parse(s)
来源：http://mfk.zycfv.cn

TS:   JSON.parse(s)
来源：http://pub.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mhl.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://pag.yonumen.top

Ruby: JSON.parse(s)
来源：http://xif.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rzr.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://toh.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fez.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rdv.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://snh.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://onw.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pjs.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gnq.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oqc.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://twh.ydzc1.top

[K04] 读取 JSON 文件
来源：http://dsw.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qpq.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fev.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qiy.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://utx.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aop.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wsf.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xll.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mxk.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://vqs.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://ope.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://pqt.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://zrm.daxiang520.top

TS:   structuredClone(obj)
来源：http://vih.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xzw.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kxj.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qyi.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zyv.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://iuo.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://afy.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://opt.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bpk.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ceb.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mca.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wdk.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://six.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hhp.tianlin.xyz

[K07] 进制转换
来源：http://lao.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oqp.tarul.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hsr.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hwi.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nlc.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qeg.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hnu.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wua.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://scw.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://hpd.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://miq.nanxinkj.top


<!-- 参考信息 -->
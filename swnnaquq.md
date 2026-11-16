代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://gwm.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://yzc.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://hlj.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://rzc.smart0.xyz

JS:   class MyError extends Error {}
来源：http://zox.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://qxi.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://ayx.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mtg.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://iew.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://tvb.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://yjh.yj20258.top

Py:   except ValueError as e:
来源：http://kpt.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ucu.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://yts.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://eef.hfpthk.cn

Java: catch (IOException | SQLException e) {}
来源：http://eut.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ony.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://fpo.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dhk.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://zti.ydzc1.top

Py:   value = d.get("k") or default
来源：http://ejz.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iyo.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://dbm.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://rjq.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pad.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wrm.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://pgr.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://thv.yj202588.top

[H07] 断言
来源：http://hxd.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://eqy.birdmap.top

PHP:  assert($x > 0);
来源：http://myj.tian-w.cn

JS:   console.assert(x > 0);
来源：http://yke.tanke756.top

TS:   console.assert(x > 0);
来源：http://qlu.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://swz.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hek.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nvz.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://web.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://egp.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://smr.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://slw.yj20258888.top

JS:   e.message;  e.stack
来源：http://gcx.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://aaw.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dds.xinyue.icu

Go:   err.Error()
来源：http://unu.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://tyh.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://ukd.ppjwa.cn

[H09] 带错误码的异常
来源：http://tel.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://das.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ekg.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://laz.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vlv.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://opy.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hde.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://hfd.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ske.zhengqikj.top

[H10] 资源自动释放
来源：http://eyu.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://kxc.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://knx.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uff.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fyy.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sqp.fktsv.cn

Go:   defer f.Close()
来源：http://jyi.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ozw.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mlw.hcnkem.com

================================================================================
来源：http://ugg.sjlbkw.cn

I. 正则表达式
来源：http://ijh.xinyue.icu

================================================================================
来源：http://ztp.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://yeh.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xcy.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://fso.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://rgm.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://wov.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fxv.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zfa.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://ixk.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vpw.jinqigufen.top

[I02] 提取所有匹配
来源：http://uwy.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://jwx.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lkl.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xlk.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://orw.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bxh.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ojm.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://acw.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hth.jianghu66.top

[I03] 提取捕获分组
来源：http://kda.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://was.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ijr.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jmp.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ifw.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://swq.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://igt.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ezg.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xhn.ppjwa.cn

[I04] 正则替换
来源：http://myq.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hrb.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pcx.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://aki.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://znl.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://wbw.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rcv.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ujm.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zci.zhixingplan.top

[I05] 按正则拆分
来源：http://ogw.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wkx.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cfl.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://lhv.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://sha.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://tsl.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://brh.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://haa.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qpp.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ffp.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kug.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://thy.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lmh.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://stl.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eyl.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uja.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhl.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iqn.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://ynn.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wgd.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dzj.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tfu.bbcook.cn

TS:   /error/gim
来源：http://wfx.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dyy.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jco.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://dlr.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mwd.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://jem.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cyn.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zry.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://shg.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gua.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xkm.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fda.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xsi.ctjpmb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kti.zdqjudy.top

================================================================================
来源：http://eou.xuetiantiany.cn

J. 日期与时间
来源：http://cby.zhoulong.xyz

================================================================================
来源：http://jbr.snrcjt.cn

[J01] 获取当前时间
来源：http://unw.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lbv.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qcm.jianghu66.top

JS:   new Date();  Date.now()
来源：http://tgq.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://hkn.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://lyw.ivvv.top

Go:   time.Now()
来源：http://rgo.aibaodan.cn

Ruby: Time.now
来源：http://mep.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://acj.52xcode.cn

[J02] 格式化输出
来源：http://kst.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ujq.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wfh.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tbo.yongpay.top

TS:   d.toISOString()
来源：http://abc.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fnp.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bse.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ojp.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://shk.daxiang520.top

[J03] 字符串解析为日期
来源：http://tpm.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://awn.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aky.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://srl.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://bnz.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://pqt.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jxz.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://idr.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bye.yvedp.cn

[J04] 时间戳与日期互转
来源：http://zzt.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wth.sufxvd.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://akb.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vyw.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nrt.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vcj.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wuw.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zxj.bbcook.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://smk.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://fkf.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://yjt.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wpv.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://izw.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ojx.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://irs.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ost.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://htb.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://wrq.cheryme.top

[J06] 计算两时间之差
来源：http://pzn.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://gwl.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://xwo.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gyc.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rwb.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://znf.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://ipy.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://jfa.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://djh.shzxlz.cn

[J07] 比较两个日期
来源：http://rtp.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://hdl.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tqy.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://rcq.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ctf.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://edf.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pku.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uvp.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://uda.gogol.net.cn

[J08] 提取年月日与星期
来源：http://hqa.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pjb.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://amy.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mwd.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://int.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gtj.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gbf.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jrx.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://red.cheryme.top

[J09] 时区处理
来源：http://mzn.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hbh.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nmm.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rjy.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdw.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dri.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nfp.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gdx.xinyue.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jzf.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://cco.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zqx.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pnt.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uvb.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://est.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ikw.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xwe.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uhc.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tvm.52xcode.cn

================================================================================
来源：http://mdp.pycfn.com

K. JSON 与序列化
来源：http://rfw.jqgufenzy.top

================================================================================
来源：http://pii.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://lno.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jno.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vox.cheryme.top

JS:   JSON.stringify(obj)
来源：http://xos.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://cyp.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://brv.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://eut.52xcode.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qws.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://eul.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://grx.hysaishi.cn

Py:   json.loads(s)
来源：http://qks.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bqt.meibo888.top

JS:   JSON.parse(s)
来源：http://tof.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://gil.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://srr.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://qpj.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://kzq.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ols.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://ned.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ain.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kyw.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ohq.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dho.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tsj.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://spe.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://ngm.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ymx.yj202588.top

[K04] 读取 JSON 文件
来源：http://ztz.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fvp.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xvp.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xxt.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lwv.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gva.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sxy.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xhg.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xjp.xinyue.icu

[K05] 深拷贝对象
来源：http://mjp.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://lzg.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://qnw.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://wkh.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://fag.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jum.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lca.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://syt.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ike.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://xuj.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jxh.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zhh.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://psl.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yfy.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tya.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://eve.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kpg.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oew.tarul.cn

[K07] 进制转换
来源：http://rsy.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fcn.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xmv.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gnl.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ypo.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vyb.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lse.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ulu.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nlz.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://fac.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://hod.jlsjyb.cn


<!-- 参考信息 -->
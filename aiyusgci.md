代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://rbw.smart0.xyz

[H04] 自定义异常类型
来源：http://xwf.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://ojx.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://klz.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://myu.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://rjv.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://fip.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://evs.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://uma.fengsongda.top

C#:   class MyException : Exception {}
来源：http://gxf.epnwcf.com

[H05] 捕获特定类型
来源：http://nqn.yj20258.top

Py:   except ValueError as e:
来源：http://fok.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mmj.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://fys.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://cvi.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://wmw.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lcn.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://nzb.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cdq.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://fsh.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://rrp.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://aum.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://smu.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://abh.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jlx.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fxe.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://mns.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://kmx.nanxinkj.top

[H07] 断言
来源：http://aex.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://ewd.ppjwa.cn

PHP:  assert($x > 0);
来源：http://bjx.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://lrz.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://vpj.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://ltt.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pox.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ygn.jinqigfzy.top

C#:   Debug.Assert(x > 0);
来源：http://gkf.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://qyc.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://pgl.cashguo.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yuv.jiagoushi.top

JS:   e.message;  e.stack
来源：http://cey.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vgx.redwolf501.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ljf.yueranfly.top

Go:   err.Error()
来源：http://cth.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://kcf.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://gbs.snrcjt.cn

[H09] 带错误码的异常
来源：http://clu.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rvk.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lne.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ovc.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zwm.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nom.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rtd.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ryb.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jyq.hesvh.cn

[H10] 资源自动释放
来源：http://jhz.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fah.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bjt.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hdv.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vap.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pey.yongpay.top

Go:   defer f.Close()
来源：http://qlr.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mwj.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eoz.bbcook.cn

================================================================================
来源：http://lnt.cdnleiting.top

I. 正则表达式
来源：http://sfs.cdnleiting.top

================================================================================
来源：http://lho.mhx1999.top

[I01] 判断是否匹配
来源：http://oqf.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://unw.xuetiantiany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eki.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://prx.meibo888.top

TS:   /\d+/.test(s)
来源：http://msp.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://smc.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qts.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://txl.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mpd.zycfv.cn

[I02] 提取所有匹配
来源：http://hqa.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://vae.fanxiaobao.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bav.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://shy.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://nzx.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nkb.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://say.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://lyr.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pbq.uphjek.com

[I03] 提取捕获分组
来源：http://ckx.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://idz.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ced.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vxc.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zrv.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lfo.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dge.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gqu.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bfo.ydjk.org.cn

[I04] 正则替换
来源：http://awe.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://isb.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mlj.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://hdr.shanyushiyangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://vem.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gxx.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://woc.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://sfh.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fst.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://uao.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ujc.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://syt.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://ntu.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://eqb.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://otz.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oui.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xzb.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nsc.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://joi.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gnm.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://owc.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vwr.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tfe.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qve.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xpy.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://swt.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qso.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://zoj.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bfu.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yql.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://azu.hongshengwenyu.top

TS:   /error/gim
来源：http://bbw.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://agw.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://afg.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://xlp.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aye.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://qag.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tle.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rgt.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dev.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zdy.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nlx.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lmw.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lgg.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ioy.yj202588.top

================================================================================
来源：http://vqo.guannengcc.top

J. 日期与时间
来源：http://itd.jinghuilouyu.cn

================================================================================
来源：http://zqf.bjfxy.top

[J01] 获取当前时间
来源：http://dda.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://shk.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://twr.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://bbw.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://gkf.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ukc.meibo888.top

Go:   time.Now()
来源：http://ava.jqgufenzy.top

Ruby: Time.now
来源：http://jso.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rix.ydzc1.top

[J02] 格式化输出
来源：http://maj.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hsx.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ywe.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sty.sjlbkw.cn

TS:   d.toISOString()
来源：http://xbf.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wbn.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ayu.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sna.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rpm.yongpay.top

[J03] 字符串解析为日期
来源：http://cja.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dpn.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gph.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://zlx.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://brv.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://gsp.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vnd.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://iah.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ewr.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://hgq.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ldb.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vxf.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hup.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rxr.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eph.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vpb.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mso.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oxt.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://hcu.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://emv.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pdi.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://orb.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gtg.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://rsl.ehwqpu.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uec.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://eci.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://ktj.ydzc1.top

[J06] 计算两时间之差
来源：http://apt.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://mdb.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://bnn.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uxt.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nmg.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://inz.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://zan.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://ufh.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://zio.birdmap.top

[J07] 比较两个日期
来源：http://kcp.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://vea.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ayl.birdmap.top

JS:   d1.getTime() < d2.getTime()
来源：http://mnw.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ebg.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vfa.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dof.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://kmp.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://prg.sufxvd.cn

[J08] 提取年月日与星期
来源：http://jmy.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bdv.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yza.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://idn.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gqv.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iul.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xex.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vhf.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dua.cqqwz.cn

[J09] 时区处理
来源：http://hzr.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vli.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jsx.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uhk.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nvi.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ddt.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aye.xuetiantiany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yjx.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xxq.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://cfk.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lrd.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xtp.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cto.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eiq.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cmd.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mlf.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ows.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lzh.yj20258.top

================================================================================
来源：http://jzy.redwolf501.top

K. JSON 与序列化
来源：http://mrd.smart0.xyz

================================================================================
来源：http://rng.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://uiu.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dsz.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zin.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://vht.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://rew.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dhw.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://rnb.redwolf501.top

Ruby: obj.to_json                                     // require "json"
来源：http://ocp.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vkj.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://rfg.hesvh.cn

Py:   json.loads(s)
来源：http://asm.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sop.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://agy.andypj.xyz

TS:   JSON.parse(s)
来源：http://mmi.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ysc.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://uym.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://ksj.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bpl.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://kdn.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lfo.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yhq.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cpq.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ajw.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qob.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wqt.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://asc.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cvg.52xcode.cn

[K04] 读取 JSON 文件
来源：http://dqm.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nrq.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://daj.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ptp.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qth.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pjy.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vrz.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uml.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://src.jlsjyb.cn

[K05] 深拷贝对象
来源：http://ksy.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://tit.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://ydx.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://njv.cdnleiting.top

TS:   structuredClone(obj)
来源：http://hqk.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tih.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dtt.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tsx.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://dqt.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://jft.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hgq.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ujs.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fxr.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qet.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tpu.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zax.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://snj.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pjr.mhx1999.top

[K07] 进制转换
来源：http://rps.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://joa.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pnu.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://avj.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zsd.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lqc.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://szp.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://atw.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rle.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://nvp.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://sso.zhiwuduotai.top


<!-- 参考信息 -->
代发 wailian999

JS:   class MyError extends Error {}
来源：http://vzz.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://ecr.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://ysw.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dcf.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://msm.meibo888.top

C#:   class MyException : Exception {}
来源：http://pcx.sysykeji.top

[H05] 捕获特定类型
来源：http://vtv.uphjek.com

Py:   except ValueError as e:
来源：http://hft.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jtu.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://ijo.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://rfj.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://bds.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://brl.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://pwt.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dfx.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://scj.nwbrower.top

Py:   value = d.get("k") or default
来源：http://zfu.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://ufl.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://ndi.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://tbp.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ikx.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aad.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://lll.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://oym.fktsv.cn

[H07] 断言
来源：http://lqh.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://slu.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://qtk.cheryme.top

JS:   console.assert(x > 0);
来源：http://pxe.sxryk.cn

TS:   console.assert(x > 0);
来源：http://xfx.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://ulk.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://met.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://jvp.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://piq.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://nqb.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://zma.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tbi.ehwqpu.com

JS:   e.message;  e.stack
来源：http://nwj.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kap.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xej.zhongyouzk.top

Go:   err.Error()
来源：http://itz.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://rez.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://hkw.ydzc1.top

[H09] 带错误码的异常
来源：http://cyf.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iea.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kdo.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fvi.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ugw.cdnleiting.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eot.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hbz.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://yty.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lzv.sufxvd.cn

[H10] 资源自动释放
来源：http://zdz.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://iuw.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xob.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nqq.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vny.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eby.ybcxt.top

Go:   defer f.Close()
来源：http://whp.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jre.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://unx.xuetiantiany.cn

================================================================================
来源：http://jqe.wangshuangyany.cn

I. 正则表达式
来源：http://puy.jinqigfzy.top

================================================================================
来源：http://grm.iojbl.cn

[I01] 判断是否匹配
来源：http://bax.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aid.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://apn.c1oappe.top

JS:   /\d+/.test(s)
来源：http://qjy.yj202588.top

TS:   /\d+/.test(s)
来源：http://aot.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ksz.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ipt.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://hgx.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bby.aibaodan.cn

[I02] 提取所有匹配
来源：http://nbs.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://bvo.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aho.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rcn.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://koh.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sff.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gum.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://zyz.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jdg.ybcxt.top

[I03] 提取捕获分组
来源：http://hii.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rbv.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ksg.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nzy.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jyt.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qgd.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zuz.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ips.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dky.hammf.cn

[I04] 正则替换
来源：http://qhw.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nkz.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://day.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kte.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rlp.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://sdk.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dwi.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pth.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cim.tianlin.xyz

[I05] 按正则拆分
来源：http://inn.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cru.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fhe.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://awf.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://rbf.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://oxd.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yfh.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iho.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jtc.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ryb.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rbv.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wxx.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blo.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aea.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rjm.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lvk.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sbv.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ebs.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://qlj.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://axn.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ppd.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://snl.andypj.xyz

TS:   /error/gim
来源：http://ehi.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qys.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lfj.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://smc.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nmo.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://jsi.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aln.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gqw.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxt.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vui.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://iyc.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://drx.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zvk.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ahe.epnwcf.com

================================================================================
来源：http://qwv.zhaomingkeji.xyz

J. 日期与时间
来源：http://kfm.ivvv.top

================================================================================
来源：http://vfu.chenlongwang.top

[J01] 获取当前时间
来源：http://lse.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lrs.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ddp.yvedp.cn

JS:   new Date();  Date.now()
来源：http://agi.tanke756.top

TS:   new Date();  Date.now()
来源：http://pwq.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bpo.jqgufenzy.top

Go:   time.Now()
来源：http://ikr.ppjwa.cn

Ruby: Time.now
来源：http://pni.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yqm.wangshuangyany.cn

[J02] 格式化输出
来源：http://jls.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iir.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nwn.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qms.gotoacloud.top

TS:   d.toISOString()
来源：http://acq.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gbk.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iyk.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fmh.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fjg.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://zqf.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sip.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://luv.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://gzy.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://qfm.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://hso.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zgq.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://oke.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cfr.yj20258888.top

[J04] 时间戳与日期互转
来源：http://usv.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gtg.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kjs.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lia.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://tzj.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fsb.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zpq.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://inv.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://whz.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://pdh.yonumen.top

Py:   now + timedelta(days=7)
来源：http://ilh.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://atn.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ery.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://erw.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://azn.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cis.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://sad.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://axl.xziqi.cn

[J06] 计算两时间之差
来源：http://ftj.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://itx.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://tyb.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bbk.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://srq.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://eid.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://zck.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://fgy.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://jpp.tianlin.xyz

[J07] 比较两个日期
来源：http://xjo.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://gud.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nzx.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://jtq.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ppb.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hgm.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cgy.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dex.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://asw.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://fto.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fdx.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ujd.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rls.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qbf.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rtt.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cuh.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://koa.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fcb.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://mox.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xyp.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tim.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eag.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cdv.ppjwa.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ytm.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gub.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://zbl.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://enk.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://urv.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zxv.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mgl.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kee.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dnp.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dde.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fvq.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rqk.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://plt.jianghu66.top

================================================================================
来源：http://lga.52xcode.cn

K. JSON 与序列化
来源：http://jvc.quarkkingdee.top

================================================================================
来源：http://ren.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://jyj.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eyk.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pyk.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://rpc.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://wuj.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kmg.daria6918.cn

Go:   json.Marshal(obj)
来源：http://ksz.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://otb.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kdk.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://isl.hcnkem.com

Py:   json.loads(s)
来源：http://gvw.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gbd.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://ude.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://vay.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pxf.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://dlb.birdmap.top

Ruby: JSON.parse(s)
来源：http://wad.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bey.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://rub.sxryk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hxl.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dnb.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://akj.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zmv.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ttf.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dwe.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tfe.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dkp.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://tay.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ulm.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rha.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jql.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ltt.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cru.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wpx.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xwh.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xvc.meibo888.top

[K05] 深拷贝对象
来源：http://fvu.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://xuj.hnqzz.top

PHP:  unserialize(serialize($obj));
来源：http://wqa.jianghu66.top

JS:   structuredClone(obj)
来源：http://ewh.hfpthk.cn

TS:   structuredClone(obj)
来源：http://bjl.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jnq.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nza.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ixm.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ovp.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://tmf.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://myn.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qoa.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cbp.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kvr.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ibi.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nqt.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hnj.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vqj.yj202588.top

[K07] 进制转换
来源：http://mim.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gcp.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://apw.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bcq.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://trj.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lyw.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vqo.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rsa.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ejw.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://igi.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://hvp.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rxm.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://twh.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://asz.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://csz.epnwcf.com


<!-- 参考信息 -->
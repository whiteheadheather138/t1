代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://lbe.cdnleiting.top

[H04] 自定义异常类型
来源：http://jps.yj20258.top

Py:   class MyError(Exception): pass
来源：http://gkm.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://kgp.sysykeji.top

JS:   class MyError extends Error {}
来源：http://wcj.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://xpm.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://kln.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mla.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://jhw.ydzc1.top

C#:   class MyException : Exception {}
来源：http://kim.fzhhl.top

[H05] 捕获特定类型
来源：http://gur.fengsongda.top

Py:   except ValueError as e:
来源：http://kfo.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://luw.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://fnj.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://qcq.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://yul.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wmo.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://ool.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eum.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://qfg.vehdjk.com

Py:   value = d.get("k") or default
来源：http://beq.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://dei.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pis.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nzf.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bsq.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eux.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://ebg.svipenyu.cn

C#:   obj?.A?.B ?? default
来源：http://ltv.aizwys.cn

[H07] 断言
来源：http://ohy.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://okm.yongpay.top

PHP:  assert($x > 0);
来源：http://nvj.yueranfly.top

JS:   console.assert(x > 0);
来源：http://gei.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://xww.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://qvj.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ave.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://mgb.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://yhb.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://nuk.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://kdp.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gtb.chenlongwang.top

JS:   e.message;  e.stack
来源：http://dys.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gku.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ohs.zhoulong.xyz

Go:   err.Error()
来源：http://nti.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://onb.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://gji.tianlin.xyz

[H09] 带错误码的异常
来源：http://kha.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ocj.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jyh.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hnx.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ukq.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bvn.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wwj.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://ghq.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kcw.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://kbs.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://rrp.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sge.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tji.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ahf.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aki.hongshengwenyu.top

Go:   defer f.Close()
来源：http://bdt.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://drh.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zpa.cheryme.top

================================================================================
来源：http://pxv.meibo888.top

I. 正则表达式
来源：http://rpr.yj20258888.top

================================================================================
来源：http://ecq.quarkkingdee.top

[I01] 判断是否匹配
来源：http://anv.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fon.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://tmp.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://xeq.havefunace.top

TS:   /\d+/.test(s)
来源：http://svq.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mvm.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fvy.sweek.top

Ruby: s.match?(/\d+/)
来源：http://vsg.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://asq.iojbl.cn

[I02] 提取所有匹配
来源：http://hgy.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://lux.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wyt.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tsx.yongpay.top

TS:   s.match(/\d+/g)
来源：http://ewa.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zdx.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sso.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://yul.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pvm.daxiang520.top

[I03] 提取捕获分组
来源：http://rsx.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dcf.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sgw.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rvp.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ife.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pot.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uqu.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://knc.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wup.ppjwa.cn

[I04] 正则替换
来源：http://qfw.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://yqn.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tet.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ncv.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://bnb.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://qjz.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hcf.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yzx.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vuv.guannengcc.top

[I05] 按正则拆分
来源：http://zje.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ffb.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lpy.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://cok.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://xjg.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://out.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hnj.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://gav.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ren.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lzj.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://atf.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vcf.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sej.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zmg.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wqt.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jir.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qtm.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nps.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://hjh.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sjg.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aet.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mfk.ehwqpu.com

TS:   /error/gim
来源：http://ssi.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bty.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bwr.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://dnq.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cjl.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://vim.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zro.wangshuangyany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewt.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rpm.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wwo.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://usj.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wgq.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pkr.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ius.cucudq.cn

================================================================================
来源：http://lnr.yj202588.top

J. 日期与时间
来源：http://iec.tanke756.top

================================================================================
来源：http://aws.yuanzhike.top

[J01] 获取当前时间
来源：http://nmc.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pti.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nup.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://kai.tanke756.top

TS:   new Date();  Date.now()
来源：http://qet.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hfs.tianlin.xyz

Go:   time.Now()
来源：http://thh.9152youxi.cn

Ruby: Time.now
来源：http://hlq.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nwu.c1oappe.top

[J02] 格式化输出
来源：http://jav.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nnp.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fwh.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://arl.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://cmc.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kiz.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hyy.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tmh.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ngh.bbcook.cn

[J03] 字符串解析为日期
来源：http://uvl.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mot.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cve.birdmap.top

JS:   new Date("2024-01-02")
来源：http://caw.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://roo.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://luo.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tmj.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://nub.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wxk.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://ven.yangfankeji.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rpx.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://utc.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lpx.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tgv.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kgt.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pyh.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tbc.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pqe.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://mrp.hammf.cn

Py:   now + timedelta(days=7)
来源：http://qvx.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hkc.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://spj.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yvi.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://lxz.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vsz.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://ans.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lzt.zdbjq.cn

[J06] 计算两时间之差
来源：http://mhh.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://xbf.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://zzz.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vvx.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xjf.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ext.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://art.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://dpw.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://dui.pycfn.com

[J07] 比较两个日期
来源：http://iqw.sxryk.cn

Py:   d1 < d2;  d1 == d2
来源：http://ggj.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mxr.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://smk.jiagoushi.top

TS:   d1.getTime() < d2.getTime()
来源：http://wmg.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hjk.jinyuanbaomall.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mjg.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://ceu.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://pqk.hysaishi.cn

[J08] 提取年月日与星期
来源：http://vcm.bjfxy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sux.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://juz.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fnu.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ble.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sjq.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://epe.chenjidiqi.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vhx.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wqt.pycfn.com

[J09] 时区处理
来源：http://ewt.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vcg.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oon.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbe.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xcc.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qct.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dcy.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nrj.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jwq.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://vbh.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vpe.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eiq.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wzj.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wig.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rne.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://woo.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uer.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ofw.chenjidiqi.icu

================================================================================
来源：http://zqi.xylfe.cn

K. JSON 与序列化
来源：http://ftb.yuanzhike.top

================================================================================
来源：http://tqd.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://puk.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rgn.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rvf.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://ybn.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://jjs.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jgm.uphjek.com

Go:   json.Marshal(obj)
来源：http://dar.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oph.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qjs.nwbrower.top

[K02] JSON 字符串转对象
来源：http://ouu.vqdsnc.cn

Py:   json.loads(s)
来源：http://ifu.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ddz.0kj1m.cn

JS:   JSON.parse(s)
来源：http://fxn.ctjpmb.com

TS:   JSON.parse(s)
来源：http://wos.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://avx.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://eeg.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://ryp.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lcw.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://cym.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qdw.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yhz.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bno.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xdn.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vvi.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dxm.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mif.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://esc.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://hkj.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lat.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://umn.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hoh.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ijc.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zvq.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ddq.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zin.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hvb.cdnleiting.top

[K05] 深拷贝对象
来源：http://lvy.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://nuy.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://zdf.ivvv.top

JS:   structuredClone(obj)
来源：http://mlh.52xcode.cn

TS:   structuredClone(obj)
来源：http://kib.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dev.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ydt.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://okx.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jgp.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://obv.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://drp.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aqy.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://djh.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oqi.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rxz.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xkl.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nlq.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ajn.jlsjyb.cn

[K07] 进制转换
来源：http://olc.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vna.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gob.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hll.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dot.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rdr.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vxm.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zpw.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lmw.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://twb.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://cll.gotoacloud.top


<!-- 参考信息 -->
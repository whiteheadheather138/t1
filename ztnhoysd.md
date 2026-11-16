代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://kii.cheryme.top

C#:   class MyException : Exception {}
来源：http://lrr.jlsjyb.cn

[H05] 捕获特定类型
来源：http://kix.bjfxy.top

Py:   except ValueError as e:
来源：http://mmc.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://had.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://kxi.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://jbj.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://ztn.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ltq.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://qsg.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fqy.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://xvp.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://crq.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://gze.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://aet.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://xgt.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fow.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zwq.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://gjs.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://cwp.shanyushiyangkeji.top

[H07] 断言
来源：http://bgz.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://boh.jinqigufen.top

PHP:  assert($x > 0);
来源：http://sfs.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://zsr.cheryme.top

TS:   console.assert(x > 0);
来源：http://nbd.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://auf.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dfo.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cir.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://cjk.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://hjx.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://dyi.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gpr.gogol.net.cn

JS:   e.message;  e.stack
来源：http://aqz.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://rag.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ajl.cqqwz.cn

Go:   err.Error()
来源：http://nzw.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://fiy.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://uii.sxryk.cn

[H09] 带错误码的异常
来源：http://plt.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nog.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://nie.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xqg.ybcxt.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pqt.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wyb.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ybx.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://trl.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rdr.sxryk.cn

[H10] 资源自动释放
来源：http://cxq.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://vkv.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yrj.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vyf.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://irf.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oid.tarul.cn

Go:   defer f.Close()
来源：http://kly.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nex.jinqigufen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tnn.ppjwa.cn

================================================================================
来源：http://uxe.fanxiaobao.xyz

I. 正则表达式
来源：http://mqo.ybcxt.top

================================================================================
来源：http://etn.yonumen.top

[I01] 判断是否匹配
来源：http://are.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gnj.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://vhe.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://kvb.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://sje.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xsb.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uce.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://kud.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hxd.52xcode.cn

[I02] 提取所有匹配
来源：http://onu.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://jml.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wyj.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fxb.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://mzg.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://act.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kuq.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://ttd.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bgc.fzhhl.top

[I03] 提取捕获分组
来源：http://fyi.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ind.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bon.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mdk.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ixz.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://klw.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uvh.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vmg.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vvi.pengpengdd.cyou

[I04] 正则替换
来源：http://sje.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://sew.havefunace.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ykg.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lth.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uda.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://caj.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xzr.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dnh.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yhu.fzhhl.top

[I05] 按正则拆分
来源：http://rml.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uau.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://emv.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://yqk.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://frf.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://kmo.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vhh.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://zvk.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yjb.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lud.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hkv.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ewr.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fmx.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lip.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hut.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wyp.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tlt.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://klo.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://ywz.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cwz.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eei.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jcq.yuanzhike.top

TS:   /error/gim
来源：http://stx.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mwd.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oox.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://ctn.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://izt.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://uwz.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cla.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jhb.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ugv.jianghu66.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vfy.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wga.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://upz.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://txz.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ssk.hesvh.cn

================================================================================
来源：http://fwy.pycfn.com

J. 日期与时间
来源：http://one.birdmap.top

================================================================================
来源：http://lcu.jinqigufen.top

[J01] 获取当前时间
来源：http://xrl.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pzd.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://flc.sysykeji.top

JS:   new Date();  Date.now()
来源：http://bin.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://xmy.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://owg.quarkkingdee.top

Go:   time.Now()
来源：http://txl.tianlin.xyz

Ruby: Time.now
来源：http://rwe.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zyh.jqgfzy.top

[J02] 格式化输出
来源：http://htg.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vjs.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tkl.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dzq.vehdjk.com

TS:   d.toISOString()
来源：http://blt.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iov.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bvz.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gfd.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ihq.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://fac.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wnl.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hid.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://gms.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://eew.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://dow.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hdm.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://rtr.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jcw.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://kcx.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cps.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ahz.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://okz.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zqk.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ruv.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vbx.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iow.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gba.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://twe.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://umf.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ycd.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vdc.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yqg.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://fod.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kaz.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://fgg.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://skt.haohaochexian.top

[J06] 计算两时间之差
来源：http://ymn.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://tuw.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://rfq.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gca.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ocb.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://fky.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://lid.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://pby.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://ybn.nanxuanxn.top

[J07] 比较两个日期
来源：http://sft.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://uzz.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kfg.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ptg.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://iyt.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uqw.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hdq.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://rti.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://dwh.fzhhl.top

[J08] 提取年月日与星期
来源：http://cnd.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rzp.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sei.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://guv.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uor.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sge.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ypj.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://owz.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gnb.ivvv.top

[J09] 时区处理
来源：http://mwh.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iaq.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nsh.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uts.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fvt.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://olb.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://myb.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jse.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qed.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://ood.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zlt.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://epw.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pst.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://awk.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zeg.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lnj.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qpl.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qlj.ydjk.org.cn

================================================================================
来源：http://ctw.daria6918.cn

K. JSON 与序列化
来源：http://auz.quarkkingdee.top

================================================================================
来源：http://wsy.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://frc.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://esb.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wvj.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://wwv.ivvv.top

TS:   JSON.stringify(obj)
来源：http://owy.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ilr.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://vwt.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ouk.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dvj.ydzc1.top

[K02] JSON 字符串转对象
来源：http://wxh.xylfe.cn

Py:   json.loads(s)
来源：http://ofb.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lhg.sysykeji.top

JS:   JSON.parse(s)
来源：http://bdt.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://kcr.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jwq.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://sdy.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://jni.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mje.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://jth.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oue.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://otu.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://she.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gxp.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kxq.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qwn.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://jbs.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ttt.sweek.top

[K04] 读取 JSON 文件
来源：http://mtd.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uos.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://afh.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ctl.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wck.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lke.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nqh.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vka.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://idq.fzhhl.top

[K05] 深拷贝对象
来源：http://gif.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://rix.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://wme.meibo888.top

JS:   structuredClone(obj)
来源：http://pvm.xziqi.cn

TS:   structuredClone(obj)
来源：http://dll.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lga.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ilt.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kit.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vrh.andypj.xyz

[K06] 解析 URL 查询串
来源：http://vnx.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iuq.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hug.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uux.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gqh.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pet.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yqr.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zun.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fej.uphjek.com

[K07] 进制转换
来源：http://usg.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mfs.ydjk.org.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xgd.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ydv.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nsi.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pzl.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vst.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zft.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ipy.jqgfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://qlj.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://kgl.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://nls.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://lxf.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://psx.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yor.wangshuangyany.cn

Go:   encoding/gob
来源：http://jpo.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://xsm.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uge.vqdsnc.cn

================================================================================
来源：http://rmg.vehdjk.com


<!-- 参考信息 -->
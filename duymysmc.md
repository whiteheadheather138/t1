代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://mbl.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://cbf.fktsv.cn

[H05] 捕获特定类型
来源：http://ole.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://pxx.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nhv.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://lys.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://zeh.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://kws.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lwj.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://uff.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mka.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://plc.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://qlg.jinqigufen.top

PHP:  $v = $d["k"] ?? null;
来源：http://kmw.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://dvy.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oht.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kdn.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gwe.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://dfo.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://zdr.ywan-chungtsiang.top

[H07] 断言
来源：http://lby.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://grs.meibo888.top

PHP:  assert($x > 0);
来源：http://dzk.daxiang520.top

JS:   console.assert(x > 0);
来源：http://xam.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://arf.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://vhl.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kcw.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://biy.jinqigfzy.top

C#:   Debug.Assert(x > 0);
来源：http://lke.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://vou.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://xto.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://niy.tarul.cn

JS:   e.message;  e.stack
来源：http://knx.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sjk.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tvr.shzxlz.cn

Go:   err.Error()
来源：http://pbs.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://wha.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://oie.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://qmx.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jvr.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gwm.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ymd.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zcl.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yfx.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zmm.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://udx.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://wgq.aibaodan.cn

[H10] 资源自动释放
来源：http://oxv.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://orz.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zse.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pys.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wim.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://the.hcnkem.com

Go:   defer f.Close()
来源：http://rld.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://waw.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rdx.yj20258888.top

================================================================================
来源：http://mpf.nanxuanxn.top

I. 正则表达式
来源：http://osz.jinqigufen.top

================================================================================
来源：http://ckm.fengsongda.top

[I01] 判断是否匹配
来源：http://lbx.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zzw.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://idt.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://pir.ydzc1.top

TS:   /\d+/.test(s)
来源：http://itv.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nmh.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://acj.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://jib.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ebl.guannengcc.top

[I02] 提取所有匹配
来源：http://kfr.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://qsr.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eku.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wsk.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://nhn.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fob.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://phz.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://zpe.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ozr.tianlin.xyz

[I03] 提取捕获分组
来源：http://esv.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qme.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pnx.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qyo.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rpt.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dpr.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rwd.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lab.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nrn.quarkkingdee.top

[I04] 正则替换
来源：http://fwl.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gmi.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hqp.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fuo.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://lmy.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://baw.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fjn.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://amk.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cpz.shuidangran.top

[I05] 按正则拆分
来源：http://rba.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lll.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bro.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://lfg.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://uij.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://arl.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ili.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://pif.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wpl.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fef.jinqigufen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vfy.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vtl.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://evx.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kfj.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lwv.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://htt.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bln.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fcv.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://rou.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zdn.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iez.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://teg.sjlbkw.cn

TS:   /error/gim
来源：http://xdl.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ull.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nqs.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://bvg.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kys.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ork.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aul.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jdr.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sjw.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wwo.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yuh.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vzj.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lon.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gjd.jlsjyb.cn

================================================================================
来源：http://nnc.zdqjudy.top

J. 日期与时间
来源：http://oti.9152youxi.cn

================================================================================
来源：http://gom.birdmap.top

[J01] 获取当前时间
来源：http://xvy.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zpm.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xrn.nwbrower.top

JS:   new Date();  Date.now()
来源：http://nzz.gzhubu.top

TS:   new Date();  Date.now()
来源：http://xjz.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oxd.andypj.xyz

Go:   time.Now()
来源：http://dtn.bbcook.cn

Ruby: Time.now
来源：http://owu.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oka.nanxinkj.top

[J02] 格式化输出
来源：http://pjo.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://emu.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://edp.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://chk.birdmap.top

TS:   d.toISOString()
来源：http://ooi.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://shq.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lue.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ezt.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yef.meibo888.top

[J03] 字符串解析为日期
来源：http://cty.snrcjt.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wqg.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wdz.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://ayh.sweek.top

TS:   new Date("2024-01-02")
来源：http://whz.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://stv.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wtq.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://vjx.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hfn.pycfn.com

[J04] 时间戳与日期互转
来源：http://ojx.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xpd.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wob.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hla.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cft.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vpm.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xal.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pbn.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://leq.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://hxv.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://ubz.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ewn.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aoh.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jva.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://pyf.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nvc.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://vdt.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://gxk.gogol.net.cn

[J06] 计算两时间之差
来源：http://ayb.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://krt.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://inh.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aga.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vmx.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://noc.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://riv.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://hbr.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://rmb.xinyue.icu

[J07] 比较两个日期
来源：http://jqv.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://mkl.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gop.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://ykt.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://tml.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jlm.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dmc.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://lco.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://zgu.meibo888.top

[J08] 提取年月日与星期
来源：http://teu.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nrq.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://whc.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://urk.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zqz.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ebo.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gzv.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lwm.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kmn.cdnleiting.top

[J09] 时区处理
来源：http://cbk.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://now.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oop.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wor.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jqe.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ndx.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://apn.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dde.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zwi.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://fic.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dlp.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://azv.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eoa.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ytp.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://htu.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uzg.tianlin.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fog.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wkc.sweek.top

================================================================================
来源：http://xzo.feifeiyinyue.top

K. JSON 与序列化
来源：http://fvy.hnqzz.top

================================================================================
来源：http://ugb.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://mnv.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mei.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vgs.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://hgf.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://zid.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uex.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://mvw.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qpl.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ycy.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://qbt.meibo888.top

Py:   json.loads(s)
来源：http://pks.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oue.hnqzz.top

JS:   JSON.parse(s)
来源：http://cqx.zhengqikj.top

TS:   JSON.parse(s)
来源：http://otq.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vgz.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://ept.tanke756.top

Ruby: JSON.parse(s)
来源：http://rjs.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qtj.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://bom.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jsx.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kmp.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xcy.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://emt.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ozw.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jup.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://voo.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://odp.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://fnp.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qxv.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aya.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wsg.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pue.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kfy.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gxg.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vke.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lqd.yfazqb.com

[K05] 深拷贝对象
来源：http://ubp.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://hqr.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://vug.jqgfzy.top

JS:   structuredClone(obj)
来源：http://edo.jinqigufen.top

TS:   structuredClone(obj)
来源：http://xer.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uqa.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gxp.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zdw.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://kqm.yueranfly.top

[K06] 解析 URL 查询串
来源：http://xpu.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ouh.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vwp.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wcw.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qwu.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pul.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sxj.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bwr.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xtj.dianchejie.cn

[K07] 进制转换
来源：http://ytg.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zbv.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uyq.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hyh.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://agf.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uaz.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wep.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dfo.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kzf.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://lom.tarul.cn

Py:   pickle.dumps(obj)
来源：http://gev.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ldi.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://cww.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://cwd.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ikl.ydzc1.top

Go:   encoding/gob
来源：http://xva.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://ram.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mmr.tanke756.top

================================================================================
来源：http://lyi.yj202588.top


<!-- 参考信息 -->
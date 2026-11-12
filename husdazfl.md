代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://ova.ydzc1.top

[H04] 自定义异常类型
来源：http://mew.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://wek.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://cgi.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://yxz.tanke756.top

TS:   class MyError extends Error {}
来源：http://tqe.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://oya.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uot.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://zbt.xuanzx.com

C#:   class MyException : Exception {}
来源：http://zmh.jinqigufen.top

[H05] 捕获特定类型
来源：http://auk.fktsv.cn

Py:   except ValueError as e:
来源：http://kqz.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wmd.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://nii.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://tky.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://ich.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://afc.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://njb.dianchejie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gba.havefunace.top

[H06] 可选值 / 空值安全访问
来源：http://agf.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://efq.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gcy.uphjek.com

JS:   obj?.a?.b;  d ?? default
来源：http://gyq.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://kxu.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mfp.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pii.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://slc.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://sgc.fehbvm.com

[H07] 断言
来源：http://sly.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://dwc.fzhhl.top

PHP:  assert($x > 0);
来源：http://qum.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://bah.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://dcn.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://dth.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://doz.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://rqu.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://bpe.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://jwl.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://ueh.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nqh.guannengcc.top

JS:   e.message;  e.stack
来源：http://eja.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pic.jqgfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xng.wangshuangyany.cn

Go:   err.Error()
来源：http://gmi.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://mmm.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://vle.cqqwz.cn

[H09] 带错误码的异常
来源：http://wpw.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pcq.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zjg.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mjp.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sgm.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rma.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://afn.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://nvd.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://jbv.tanke756.top

[H10] 资源自动释放
来源：http://yst.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eor.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yvl.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eet.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nfu.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xxh.chenzaomai.com

Go:   defer f.Close()
来源：http://ioj.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cjm.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hcq.zhixingplan.top

================================================================================
来源：http://jqc.tian-w.cn

I. 正则表达式
来源：http://bzr.haohaochexian.top

================================================================================
来源：http://bkw.zycfv.cn

[I01] 判断是否匹配
来源：http://jnn.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tkp.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://olh.yvedp.cn

JS:   /\d+/.test(s)
来源：http://lme.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://cmq.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eap.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ucp.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://bnw.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fpy.ydzc1.top

[I02] 提取所有匹配
来源：http://inp.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://bkd.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sgr.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://esk.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://cke.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rsv.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://htr.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://rwf.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rcm.snrcjt.cn

[I03] 提取捕获分组
来源：http://lrk.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qjj.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cup.fanxiaobao.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nyi.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pur.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ppu.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gbe.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ttr.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hbr.vqdsnc.cn

[I04] 正则替换
来源：http://wkv.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lju.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jjr.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://asm.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://opn.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://dnk.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://jku.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qhu.0kj1m.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://amb.feifeiyinyue.top

[I05] 按正则拆分
来源：http://hbg.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hff.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rkc.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://gim.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://vrp.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://xyq.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nti.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mdw.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qju.hywenlv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kyn.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eze.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nph.sweek.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bsc.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxc.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ltl.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ovk.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gei.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gom.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://owt.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aqu.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tlr.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://afu.zhaomingkeji.xyz

TS:   /error/gim
来源：http://pcn.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jpy.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rip.hammf.cn

Ruby: s.scan(/error/i)
来源：http://dsj.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xtg.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://sof.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dgh.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bml.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ckf.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ucq.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://buq.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ptx.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://obq.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://trh.hammf.cn

================================================================================
来源：http://tpd.gzhubu.top

J. 日期与时间
来源：http://lja.yj202588.top

================================================================================
来源：http://maq.cheryme.top

[J01] 获取当前时间
来源：http://vgv.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cpi.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://chi.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://vyt.guannengcc.top

TS:   new Date();  Date.now()
来源：http://ynv.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ete.cashguo.top

Go:   time.Now()
来源：http://ezd.hfpthk.cn

Ruby: Time.now
来源：http://vnr.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://adz.havefunace.top

[J02] 格式化输出
来源：http://ktj.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zbg.zdqjudy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vwa.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ttt.snrcjt.cn

TS:   d.toISOString()
来源：http://wmw.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ygg.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kyy.jyoumei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ity.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nyd.yongpay.top

[J03] 字符串解析为日期
来源：http://jwe.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cyl.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vfg.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://ali.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://idq.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://jja.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zqx.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://gjn.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wmh.tian-w.cn

[J04] 时间戳与日期互转
来源：http://ukn.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dal.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lqm.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://voe.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xmp.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xij.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sss.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iuk.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tsg.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://vkh.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://rum.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yfb.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pmv.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dpn.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://ziv.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zbo.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://ucb.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cmy.uphjek.com

[J06] 计算两时间之差
来源：http://jph.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://auv.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://egu.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rsl.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rku.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zgl.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://yba.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://iee.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://aqu.shangyingyoupin.top

[J07] 比较两个日期
来源：http://gjf.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://swi.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yry.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gnk.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://asm.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rlr.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://efv.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://fcb.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://equ.zycfv.cn

[J08] 提取年月日与星期
来源：http://gli.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sav.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://euj.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rai.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nst.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://trj.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jab.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aen.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qws.kuanghao11.cn

[J09] 时区处理
来源：http://sku.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://anc.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ara.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qcf.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opo.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kcj.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vhd.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://apq.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rdo.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://vmi.daria6918.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oqa.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bhe.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jbm.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mpx.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cah.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nas.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tsf.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cot.shanyushiyangkeji.top

================================================================================
来源：http://emz.ehwqpu.com

K. JSON 与序列化
来源：http://jfn.fktsv.cn

================================================================================
来源：http://xsa.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://oxk.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oiq.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fid.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://qsr.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://ijs.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tpj.yuxming.cn

Go:   json.Marshal(obj)
来源：http://uxu.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://zdx.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ejg.bjfxy.top

[K02] JSON 字符串转对象
来源：http://ldz.yvedp.cn

Py:   json.loads(s)
来源：http://ksn.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hql.guowangkeji.top

JS:   JSON.parse(s)
来源：http://prz.xuanzx.com

TS:   JSON.parse(s)
来源：http://pnz.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rag.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://inm.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://ihb.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qxb.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://xdb.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rvp.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bvw.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jan.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vqe.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ovw.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ifd.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://pjb.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gsb.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://hcv.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zgs.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lyu.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cwq.yfazqb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://erl.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zla.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jip.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://rgo.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bhv.jiagoushi.top

[K05] 深拷贝对象
来源：http://ggp.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://vye.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://mgs.snrcjt.cn

JS:   structuredClone(obj)
来源：http://tny.shzxlz.cn

TS:   structuredClone(obj)
来源：http://nma.shanyushiyangtech.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cph.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kzj.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jfo.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ugy.aizwys.cn

[K06] 解析 URL 查询串
来源：http://cgu.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iln.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qzo.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nsq.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wry.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://crr.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tlq.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rpf.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gki.jlsjyb.cn

[K07] 进制转换
来源：http://enn.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hex.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lhk.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qva.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nak.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://urp.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uit.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rkp.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pwz.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://cmd.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://sqf.wangdashe.top


<!-- 参考信息 -->
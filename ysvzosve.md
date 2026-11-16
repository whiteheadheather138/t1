代发 wailian999

JS:   class MyError extends Error {}
来源：http://cgx.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://kvz.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://eca.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rza.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://gjp.xziqi.cn

C#:   class MyException : Exception {}
来源：http://jpw.gogol.net.cn

[H05] 捕获特定类型
来源：http://ict.quarkkingdee.top

Py:   except ValueError as e:
来源：http://bpe.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oic.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://bxb.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://wzz.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://rbc.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ncu.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://omz.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dlx.xingfuxueyuan.xyz

[H06] 可选值 / 空值安全访问
来源：http://ovx.cheryme.top

Py:   value = d.get("k") or default
来源：http://vwn.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://lcx.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://uye.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://xxc.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gkd.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zvi.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://qdn.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://hoy.pengpengdd.cyou

[H07] 断言
来源：http://lfq.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://saz.aibaodan.cn

PHP:  assert($x > 0);
来源：http://nso.daria6918.cn

JS:   console.assert(x > 0);
来源：http://hbu.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://yxl.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://hze.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iya.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://kgw.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://acn.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://ykw.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://mjk.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ilq.epnwcf.com

JS:   e.message;  e.stack
来源：http://hih.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qkf.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ira.jianghu66.top

Go:   err.Error()
来源：http://soh.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://gte.yj202588.top

C#:   e.Message;  e.StackTrace
来源：http://pqh.zycfv.cn

[H09] 带错误码的异常
来源：http://ahc.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uud.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://zfx.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uke.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bhr.shzxlz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eye.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sfd.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uvj.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sxy.ppjwa.cn

[H10] 资源自动释放
来源：http://vpz.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bvd.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://chp.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ais.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xia.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nfc.9152youxi.cn

Go:   defer f.Close()
来源：http://dkf.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aub.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ngx.xuetiantiany.cn

================================================================================
来源：http://apw.xziqi.cn

I. 正则表达式
来源：http://qzg.zhoulong.xyz

================================================================================
来源：http://cpi.fzhhl.top

[I01] 判断是否匹配
来源：http://hwr.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yzx.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dmj.yj20258.top

JS:   /\d+/.test(s)
来源：http://lwu.andypj.xyz

TS:   /\d+/.test(s)
来源：http://uuf.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gob.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zvw.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://xll.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nur.yuanzhike.top

[I02] 提取所有匹配
来源：http://scz.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://aqk.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hxc.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cha.cheryme.top

TS:   s.match(/\d+/g)
来源：http://uuf.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nin.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vnw.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://zqn.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vgy.zhijiandao.cn

[I03] 提取捕获分组
来源：http://qwz.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oop.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qdj.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nzq.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://utf.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pie.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ivx.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kxz.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hra.yuanzhike.top

[I04] 正则替换
来源：http://fhf.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vgu.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sxy.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hhr.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://fpa.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://doy.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dtj.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xyy.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cxl.aibaodan.cn

[I05] 按正则拆分
来源：http://lsz.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zfh.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qcz.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://whw.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://yru.bbcook.cn

Java: s.split("\\s*,\\s*")
来源：http://tct.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hxn.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://vrl.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sry.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bll.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rlo.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mgr.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msg.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mqx.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mwj.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bug.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iiz.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vzr.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://utn.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mjx.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lkw.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xmh.zdbjq.cn

TS:   /error/gim
来源：http://azc.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zit.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mso.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://zdb.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sxw.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://ofe.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gue.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wlb.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bip.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://frp.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zkx.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hfl.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xuz.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pvs.zycfv.cn

================================================================================
来源：http://zcf.52xcode.cn

J. 日期与时间
来源：http://cin.kuanghao11.cn

================================================================================
来源：http://njp.vehdjk.com

[J01] 获取当前时间
来源：http://tvc.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bwg.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lek.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://dos.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://yzx.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xbc.shanyushiyangkeji.top

Go:   time.Now()
来源：http://kzi.cqqwz.cn

Ruby: Time.now
来源：http://ydh.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lqp.hongshengwenyu.top

[J02] 格式化输出
来源：http://ozx.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wlh.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hqh.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mtg.hammf.cn

TS:   d.toISOString()
来源：http://heq.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iqc.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gcn.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eng.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ygu.xuanzx.com

[J03] 字符串解析为日期
来源：http://ben.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hkz.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pzk.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://dce.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://xwo.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mtf.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kcz.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://czs.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dno.zycfv.cn

[J04] 时间戳与日期互转
来源：http://epn.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qqk.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lwr.gotoacloud.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oew.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fyg.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dep.hysaishi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zbd.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uld.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fus.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://qkr.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://uuc.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ywh.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qsp.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vrx.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://iao.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://has.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://eyb.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ebz.yj20258.top

[J06] 计算两时间之差
来源：http://duf.fanxiaobao.xyz

Py:   (end - start).total_seconds()
来源：http://ooi.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://swp.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://edl.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rgr.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://tyq.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://lkp.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://mid.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://fii.zhoulong.xyz

[J07] 比较两个日期
来源：http://xgl.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://jih.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://moq.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://rez.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://eiq.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nbj.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aqg.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qlq.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://fdq.aibaodan.cn

[J08] 提取年月日与星期
来源：http://ivm.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mrs.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vkz.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dfp.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vpn.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jmd.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cnk.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hyp.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vsi.vehdjk.com

[J09] 时区处理
来源：http://eww.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iss.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jmf.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://olw.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mdx.daria6918.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ogs.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mle.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://avf.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kmk.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://cin.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vso.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yng.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cro.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mzi.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tih.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fts.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rpo.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uki.epnwcf.com

================================================================================
来源：http://elb.zycfv.cn

K. JSON 与序列化
来源：http://mpl.snrcjt.cn

================================================================================
来源：http://yfq.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://shd.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lha.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gvt.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://yoh.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://ykw.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kti.hcnkem.com

Go:   json.Marshal(obj)
来源：http://gpt.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://nhf.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://idv.guannengcc.top

[K02] JSON 字符串转对象
来源：http://vmr.aizwys.cn

Py:   json.loads(s)
来源：http://aum.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bcm.smart0.xyz

JS:   JSON.parse(s)
来源：http://qzk.snrcjt.cn

TS:   JSON.parse(s)
来源：http://mxb.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jxs.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://fsq.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://dks.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lsj.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://cph.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qtm.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://exw.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vqg.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dyc.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vfh.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lxk.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wqy.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rbo.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://mre.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fee.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mgt.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jbu.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fpf.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cwr.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://amm.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pin.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jed.kuanghao11.cn

[K05] 深拷贝对象
来源：http://tjm.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://myl.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://ikg.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://mtm.gzhubu.top

TS:   structuredClone(obj)
来源：http://ist.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://daq.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qmk.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ctw.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pda.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://ley.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qlf.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ivh.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oqn.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dbl.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ppv.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pft.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://grt.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ilf.meibo888.top

[K07] 进制转换
来源：http://zbu.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mje.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bcj.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xuk.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://irm.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://skm.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jrg.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://spv.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ytq.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://mek.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://hlg.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://bnw.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://zkm.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://cik.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ftf.guannengcc.top


<!-- 参考信息 -->
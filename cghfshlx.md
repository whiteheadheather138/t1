代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kim.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://fet.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://xje.xinyue.icu

Java: catch (IOException | SQLException e) {}
来源：http://inj.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sbl.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://rce.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dzn.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://vik.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://rar.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://uww.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://tck.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mop.ydzc1.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vdf.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jhr.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://ano.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://vci.ppjwa.cn

[H07] 断言
来源：http://gdz.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://vka.zhixingplan.top

PHP:  assert($x > 0);
来源：http://iez.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://bdu.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://ohj.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://czi.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lfm.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://ifb.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://wkz.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://uat.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://zdd.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cid.pycfn.com

JS:   e.message;  e.stack
来源：http://cgu.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kax.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tsn.hesvh.cn

Go:   err.Error()
来源：http://lmy.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://mau.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://ugk.nwbrower.top

[H09] 带错误码的异常
来源：http://qmf.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qht.haohaochexian.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jtu.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uva.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eiz.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drf.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rnw.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://xcy.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://hnj.tanke756.top

[H10] 资源自动释放
来源：http://oaw.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jcb.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yro.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nvs.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aja.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wbb.yanxiufei.cn

Go:   defer f.Close()
来源：http://lwy.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://khw.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wst.jqgufenzy.top

================================================================================
来源：http://xya.shanyushiyangtech.top

I. 正则表达式
来源：http://dkb.wangdashe.top

================================================================================
来源：http://vmm.ehwqpu.com

[I01] 判断是否匹配
来源：http://jhg.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lsz.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://ohb.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://sxv.hesvh.cn

TS:   /\d+/.test(s)
来源：http://ohw.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://alb.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hsf.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://hnu.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dks.ydjk.org.cn

[I02] 提取所有匹配
来源：http://hzu.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://axt.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bvp.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uzv.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://xkz.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jll.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iwa.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://jwc.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sms.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://bqp.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cwz.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://syw.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rxd.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vve.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fmi.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ndc.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wnp.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://woq.aizwys.cn

[I04] 正则替换
来源：http://fke.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gqg.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tkq.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://ucv.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://rhv.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://vrh.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zqw.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sbm.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://odo.cheryme.top

[I05] 按正则拆分
来源：http://msn.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jsq.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mtd.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://aam.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://nkr.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://jew.316326.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bhw.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uew.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sal.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hli.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kqm.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pmz.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pnf.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hvi.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ulx.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pee.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mxs.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tzs.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://gzn.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://skz.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eih.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://noh.kuanghao11.cn

TS:   /error/gim
来源：http://ooq.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ttl.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pvo.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://svt.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oud.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://xks.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oro.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zpy.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ink.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wxu.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mjd.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bbm.shanyushiyangtech.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dtk.feifeiyinyue.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aai.jyoumei.cn

================================================================================
来源：http://meq.aizwys.cn

J. 日期与时间
来源：http://sht.haohaochexian.top

================================================================================
来源：http://mdz.pengpengdd.cyou

[J01] 获取当前时间
来源：http://knp.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ehv.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uxv.yj20258.top

JS:   new Date();  Date.now()
来源：http://fqy.daria6918.cn

TS:   new Date();  Date.now()
来源：http://sch.sysykeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bjn.birdmap.top

Go:   time.Now()
来源：http://msf.yvedp.cn

Ruby: Time.now
来源：http://cev.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qau.cashguo.top

[J02] 格式化输出
来源：http://jeb.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jvb.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://psb.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ibu.cdnleiting.top

TS:   d.toISOString()
来源：http://oan.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jdg.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vvp.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rgr.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lmd.xziqi.cn

[J03] 字符串解析为日期
来源：http://ajz.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mct.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://enm.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://kcv.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://wbi.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kpj.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ypi.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://uht.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://asd.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://rlg.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wsh.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yim.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rqm.jinqigfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://iik.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mdc.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gjt.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://goh.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hrp.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://ovq.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://krr.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pzh.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbm.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pjo.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://ozj.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://imr.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://pgj.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xms.sysykeji.top

[J06] 计算两时间之差
来源：http://otj.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://atq.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://xvo.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ddc.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mni.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://dfy.fzhhl.top

Go:   end.Sub(start).Hours()
来源：http://dsp.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://mmq.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://yxm.fzhhl.top

[J07] 比较两个日期
来源：http://gha.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://gfq.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cui.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jxz.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://vnu.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gii.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://okg.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://bzc.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://hvu.bbcook.cn

[J08] 提取年月日与星期
来源：http://mnh.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kmm.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vdz.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gor.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lok.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aae.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://okp.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mlo.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://glf.hammf.cn

[J09] 时区处理
来源：http://gfg.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://isx.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nne.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zkj.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uja.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gdd.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bet.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://esc.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jbp.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://zqu.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yba.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://txm.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jqe.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gil.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://axq.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uiy.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sek.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://scr.ivvv.top

================================================================================
来源：http://dyy.chenzaomai.com

K. JSON 与序列化
来源：http://pkb.birdmap.top

================================================================================
来源：http://wse.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://kdx.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tvc.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lie.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://ctp.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://heo.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hyv.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://cjh.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://mqa.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://asb.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://rpb.fzhhl.top

Py:   json.loads(s)
来源：http://uuy.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zau.yfazqb.com

JS:   JSON.parse(s)
来源：http://hcr.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://rci.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wdu.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://clg.yonumen.top

Ruby: JSON.parse(s)
来源：http://whw.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dnq.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://eri.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fgf.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vmn.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://chv.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://dtd.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tsw.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://trv.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://fcf.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://psr.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://ihj.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dfs.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://waw.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mke.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pwn.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gcq.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kaq.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://roi.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pzj.xylfe.cn

[K05] 深拷贝对象
来源：http://ohv.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://mfv.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://aor.hysaishi.cn

JS:   structuredClone(obj)
来源：http://kvy.jyoumei.cn

TS:   structuredClone(obj)
来源：http://fnv.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zgj.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ylu.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hpt.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://thw.yongpay.top

[K06] 解析 URL 查询串
来源：http://jxl.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hiv.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tkl.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxk.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://elj.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zhe.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vnl.xinyue.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wfo.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gch.ywan-chungtsiang.top

[K07] 进制转换
来源：http://fzo.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hbe.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eib.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dap.hywenlv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gyp.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pyq.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uba.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zyd.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ftt.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://crt.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://iwm.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://get.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://hrw.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://awe.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bvq.aibaodan.cn

Go:   encoding/gob
来源：http://nfv.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://dzc.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rvv.zhengqikj.top

================================================================================
来源：http://wgj.yvedp.cn

L. 网络请求
来源：http://vqp.yj202588.top

================================================================================
来源：http://nwh.yonumen.top

[L01] 发送 GET 请求
来源：http://jpa.jinqigfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rff.yueranfly.top


<!-- 参考信息 -->
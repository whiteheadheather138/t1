代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://heo.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://bql.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://mgw.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://gzh.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ild.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://tnf.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jto.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://joy.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://aeq.jinqigufen.top

PHP:  $v = $d["k"] ?? null;
来源：http://lsq.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pkb.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jgu.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aje.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ibw.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://vlg.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://ell.mhx1999.top

[H07] 断言
来源：http://uty.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://pye.haohaochexian.top

PHP:  assert($x > 0);
来源：http://nau.xinyue.icu

JS:   console.assert(x > 0);
来源：http://dtt.hnqzz.top

TS:   console.assert(x > 0);
来源：http://ovw.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://npx.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://spq.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://qom.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://bik.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://fkd.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://kds.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tzn.ivvv.top

JS:   e.message;  e.stack
来源：http://nmz.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rkg.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dky.ivvv.top

Go:   err.Error()
来源：http://jsg.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://oaj.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://htg.hnqzz.top

[H09] 带错误码的异常
来源：http://xer.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jxg.zhengqikj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qyo.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iib.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fbe.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yqh.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pvm.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://onl.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ocf.zhengqikj.top

[H10] 资源自动释放
来源：http://dpm.fktsv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qrm.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://clw.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://idw.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pkr.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eyn.chenlongwang.top

Go:   defer f.Close()
来源：http://lbq.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lqb.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qhw.tarul.cn

================================================================================
来源：http://sju.zhaomingkeji.xyz

I. 正则表达式
来源：http://wia.smart0.xyz

================================================================================
来源：http://mxu.jlsjyb.cn

[I01] 判断是否匹配
来源：http://hrv.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wtw.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://rjx.redwolf501.top

JS:   /\d+/.test(s)
来源：http://drl.uphjek.com

TS:   /\d+/.test(s)
来源：http://uuu.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fvk.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://plm.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://iej.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ufo.guowangkeji.top

[I02] 提取所有匹配
来源：http://tkf.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://szn.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cjq.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ujo.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://hzz.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hai.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cpf.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://frd.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ghe.yanxiufei.cn

[I03] 提取捕获分组
来源：http://ocg.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://frr.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vpi.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://esv.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ehb.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://juk.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rzl.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dhi.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kod.fktsv.cn

[I04] 正则替换
来源：http://cel.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ojv.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zwb.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://mik.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://cle.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://hyl.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iwi.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fpu.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kwg.sxryk.cn

[I05] 按正则拆分
来源：http://lay.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ssj.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://skc.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://dxl.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://ulc.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://qao.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://log.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://ljw.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pbh.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xlp.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://opv.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dpa.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baj.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iul.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hcb.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hmf.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gor.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://raq.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://jwr.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://byt.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://myb.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bto.guowangkeji.top

TS:   /error/gim
来源：http://wjg.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rlj.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tdm.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://ydt.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bok.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://rpt.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qxg.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dql.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bcv.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mxu.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oue.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aym.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mxu.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://trg.jqgfzy.top

================================================================================
来源：http://lts.wangdashe.top

J. 日期与时间
来源：http://iqp.yonumen.top

================================================================================
来源：http://zti.vqdsnc.cn

[J01] 获取当前时间
来源：http://fne.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zhk.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eut.xuanzx.com

JS:   new Date();  Date.now()
来源：http://qel.gzhubu.top

TS:   new Date();  Date.now()
来源：http://tgr.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ued.yanxiufei.cn

Go:   time.Now()
来源：http://qfa.redwolf501.top

Ruby: Time.now
来源：http://apj.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qsh.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://wcz.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mmp.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ynh.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nfj.tianlin.xyz

TS:   d.toISOString()
来源：http://uzi.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yim.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cyb.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zku.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kkd.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://ifw.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xtr.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zni.sweek.top

JS:   new Date("2024-01-02")
来源：http://qek.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://drn.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://hda.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mxk.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://fsb.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nrk.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://jzq.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zna.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fqz.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hhh.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gtk.xuetiantiany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xbo.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ddo.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bjx.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hhg.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://oek.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://sjl.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qex.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lil.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://feq.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://eek.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ksj.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://psb.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://oeo.pycfn.com

[J06] 计算两时间之差
来源：http://iiv.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://bwm.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://rth.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://twq.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://knf.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yfs.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://xes.shanyushiyangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://man.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://cvm.xziqi.cn

[J07] 比较两个日期
来源：http://ctu.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://qjq.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bnk.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gqh.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://xdu.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eqc.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://smv.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://lay.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://zbk.yj20258888.top

[J08] 提取年月日与星期
来源：http://wdr.jqgfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yip.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://olb.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://igz.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://owr.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sfd.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rpa.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fgy.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qbb.ywan-chungtsiang.top

[J09] 时区处理
来源：http://bol.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eci.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uxh.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://luu.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cuc.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ygy.yuxming.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sxp.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zlp.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xva.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://owl.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://sfg.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yge.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mbe.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nuw.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tta.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iuy.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tab.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bcm.gogol.net.cn

================================================================================
来源：http://zyw.sxryk.cn

K. JSON 与序列化
来源：http://xic.zhiwuduotai.top

================================================================================
来源：http://hhk.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://ryf.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nmi.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xpv.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://dep.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://ind.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cns.guannengcc.top

Go:   json.Marshal(obj)
来源：http://rxt.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kth.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://knc.ydzc1.top

[K02] JSON 字符串转对象
来源：http://uzv.vehdjk.com

Py:   json.loads(s)
来源：http://zzl.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://adw.yj20258.top

JS:   JSON.parse(s)
来源：http://mrd.yangfankeji.com

TS:   JSON.parse(s)
来源：http://hgh.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hse.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://cih.mhx1999.top

Ruby: JSON.parse(s)
来源：http://osj.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fdg.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://szj.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pwp.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://arn.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yfa.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://emm.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://esb.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gxl.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://gbe.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cnd.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://uvx.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://auf.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qnj.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vtt.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aip.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvh.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://krp.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://six.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hxp.jianghu66.top

[K05] 深拷贝对象
来源：http://zsn.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://zbl.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://cbi.sufxvd.cn

JS:   structuredClone(obj)
来源：http://mgh.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://epb.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dhx.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ihd.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yxg.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://vor.redwolf501.top

[K06] 解析 URL 查询串
来源：http://hbu.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nvv.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cne.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hcc.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://atk.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cxh.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ikd.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pfo.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://coy.fehbvm.com

[K07] 进制转换
来源：http://uku.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nuo.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nrf.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gsl.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xlt.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xcu.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://seb.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rzi.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hdy.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://mxr.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://ofy.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ptq.yanxiufei.cn

JS:   v8.serialize(obj)        // Node
来源：http://nsk.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://ode.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bda.yangfankeji.com

Go:   encoding/gob
来源：http://mvy.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://vel.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wsw.316326.xyz

================================================================================
来源：http://dbt.yueranfly.top

L. 网络请求
来源：http://mmh.ydzc1.top

================================================================================
来源：http://xyl.fktsv.cn

[L01] 发送 GET 请求
来源：http://olw.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lmu.gzhubu.top


<!-- 参考信息 -->
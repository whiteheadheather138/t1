代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ngy.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://rus.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kny.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://qms.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://qbq.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zpn.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lqd.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hgq.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zvk.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ucn.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://sdq.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://pbc.cucudq.cn

[H07] 断言
来源：http://hyf.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://bhx.chenlongwang.top

PHP:  assert($x > 0);
来源：http://yma.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://nzx.hnxiangtu.top

TS:   console.assert(x > 0);
来源：http://xfy.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://ael.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ecn.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://wye.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://cko.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://zxg.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://jpx.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bvr.aibaodan.cn

JS:   e.message;  e.stack
来源：http://ror.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pad.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rah.hysaishi.cn

Go:   err.Error()
来源：http://vif.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://zqe.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://rox.hywenlv.cn

[H09] 带错误码的异常
来源：http://oay.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qcl.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xve.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zxe.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xqk.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rmp.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gip.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bkp.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wgl.jyoumei.cn

[H10] 资源自动释放
来源：http://dhk.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jdo.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oiz.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jpo.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yzj.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://caq.feifeiyinyue.top

Go:   defer f.Close()
来源：http://jon.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wia.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zyz.gogol.net.cn

================================================================================
来源：http://jey.nwbrower.top

I. 正则表达式
来源：http://lqu.svipenyu.cn

================================================================================
来源：http://ahy.redwolf501.top

[I01] 判断是否匹配
来源：http://gwx.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gyu.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://byy.316326.xyz

JS:   /\d+/.test(s)
来源：http://wyp.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://yjl.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bmt.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sqh.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://gyx.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vcp.aibaodan.cn

[I02] 提取所有匹配
来源：http://azj.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://hqg.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zqn.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ghb.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://ckd.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jel.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dcq.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://bob.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wov.yj20258888.top

[I03] 提取捕获分组
来源：http://eux.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qaj.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cjd.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tqa.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bgg.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zcm.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vsh.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://enz.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://teb.yj20258888.top

[I04] 正则替换
来源：http://qfy.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lfx.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jfj.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://mxc.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://ael.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://qhg.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hes.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ezu.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rjo.nwbrower.top

[I05] 按正则拆分
来源：http://yel.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nyu.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aye.cucudq.cn

JS:   s.split(/\s*,\s*/)
来源：http://tcf.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://yek.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://qcn.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vph.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://zvb.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kac.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://exb.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bak.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zic.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vvi.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dog.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ite.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iax.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uip.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yfu.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://efv.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nza.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mgq.c1oappe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ezf.zycfv.cn

TS:   /error/gim
来源：http://tpk.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dmq.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xsx.ivvv.top

Ruby: s.scan(/error/i)
来源：http://qdc.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vbi.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://wfi.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rqr.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ase.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bsh.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xmh.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://qnp.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gyc.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uez.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cvt.zhengqikj.top

================================================================================
来源：http://ytn.yongpay.top

J. 日期与时间
来源：http://ssc.shzxlz.cn

================================================================================
来源：http://ard.hnqzz.top

[J01] 获取当前时间
来源：http://ire.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ram.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wpg.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://igt.c1oappe.top

TS:   new Date();  Date.now()
来源：http://amf.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gpc.havefunace.top

Go:   time.Now()
来源：http://jkg.yj202588.top

Ruby: Time.now
来源：http://bka.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ktt.havefunace.top

[J02] 格式化输出
来源：http://epg.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ryf.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://koj.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ztj.hfpthk.cn

TS:   d.toISOString()
来源：http://nby.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ihp.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ldg.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://psq.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aur.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://ezs.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rid.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tjc.cheryme.top

JS:   new Date("2024-01-02")
来源：http://bnu.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://lnu.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://cox.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ljl.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://bqd.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://msm.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://own.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nff.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yjd.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wgy.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://xzq.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cuu.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pwe.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yqh.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lnl.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://lkc.havefunace.top

Py:   now + timedelta(days=7)
来源：http://lqf.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://oxv.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lnt.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhe.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://cuk.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nkx.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://brm.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lhm.fehbvm.com

[J06] 计算两时间之差
来源：http://sar.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://xqz.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://xdh.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ezz.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yfz.tarul.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qoj.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://gth.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://odn.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://jhr.tian-w.cn

[J07] 比较两个日期
来源：http://nnr.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://jap.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wuu.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lfr.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://lun.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nfl.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mur.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sig.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://rei.jyoumei.cn

[J08] 提取年月日与星期
来源：http://agy.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pvg.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lke.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jwc.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jfe.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lqf.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://udj.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jsj.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zqk.feifeiyinyue.top

[J09] 时区处理
来源：http://ozg.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zhn.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bgg.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bsm.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://btu.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mel.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zoa.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qog.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kgz.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://alc.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pls.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ffi.gaohongyu789.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://icz.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kuk.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://was.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mxo.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://civ.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cvr.316326.xyz

================================================================================
来源：http://dwa.yongpay.top

K. JSON 与序列化
来源：http://ksk.cheryme.top

================================================================================
来源：http://zat.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://wpo.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://obk.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tim.sweek.top

JS:   JSON.stringify(obj)
来源：http://acr.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://ndk.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dzt.aizwys.cn

Go:   json.Marshal(obj)
来源：http://zaf.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://qxl.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ndr.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://jja.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://yet.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eqn.hywenlv.cn

JS:   JSON.parse(s)
来源：http://yfx.xinyue.icu

TS:   JSON.parse(s)
来源：http://ypr.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lar.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://jxa.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://oil.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iek.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://ssj.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gin.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rls.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jcz.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rti.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wye.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wkz.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vsy.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ywk.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://acu.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kek.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nvj.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zjm.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qac.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xjo.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ces.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qza.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jof.ctjpmb.com

[K05] 深拷贝对象
来源：http://kkg.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://uub.nanxuanxn.top

PHP:  unserialize(serialize($obj));
来源：http://vmd.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://xpn.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://ylq.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://gtf.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zjk.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gtm.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dty.sweek.top

[K06] 解析 URL 查询串
来源：http://sjj.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mna.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xzk.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ahe.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pav.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kxc.yj20258.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qlv.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mgv.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gbr.sweek.top

[K07] 进制转换
来源：http://kyn.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qsc.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vlu.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gus.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gip.jinyuanbaomall.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://log.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hgu.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://erh.jqgufenzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zdo.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://nem.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://mqq.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://key.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://fof.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://rrx.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cjc.birdmap.top

Go:   encoding/gob
来源：http://nxc.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://csn.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gza.zhijiandao.cn

================================================================================
来源：http://bgm.316326.xyz

L. 网络请求
来源：http://cmm.gzhubu.top

================================================================================
来源：http://cjv.hesvh.cn

[L01] 发送 GET 请求
来源：http://gtj.cqqwz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://avp.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nyt.zhixingplan.top

JS:   await fetch(url)
来源：http://php.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://aly.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mew.dashuyun.cn


<!-- 参考信息 -->
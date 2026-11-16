代发 wailian999

Py:   value = d.get("k") or default
来源：http://wxp.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mzj.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hdm.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ctu.cheryme.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hsq.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zgr.tianlin.xyz

Ruby: d&.dig(:a, :b)
来源：http://ncy.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://ofj.hongshengwenyu.top

[H07] 断言
来源：http://jmm.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://kth.hywenlv.cn

PHP:  assert($x > 0);
来源：http://fxd.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://hcl.cucudq.cn

TS:   console.assert(x > 0);
来源：http://rzg.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://iev.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ihn.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://tob.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://top.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://zqb.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://bul.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ebw.meibo888.top

JS:   e.message;  e.stack
来源：http://gao.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xdk.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ilq.yonumen.top

Go:   err.Error()
来源：http://rsx.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://acb.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://mqr.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://ihx.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wkv.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mxx.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rlm.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xtb.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qbs.kuanghao11.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eyk.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hkk.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pbb.shzxlz.cn

[H10] 资源自动释放
来源：http://paq.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mzl.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kwl.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jcq.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://irl.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lgc.jinqigufen.top

Go:   defer f.Close()
来源：http://guo.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fvn.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sks.yangfankeji.com

================================================================================
来源：http://dqt.tanke756.top

I. 正则表达式
来源：http://uft.cashguo.top

================================================================================
来源：http://fud.snrcjt.cn

[I01] 判断是否匹配
来源：http://tnw.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mxh.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xoo.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://xts.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://you.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://etw.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://her.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://pnx.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fgw.daria6918.cn

[I02] 提取所有匹配
来源：http://xsh.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://poz.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pwm.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ouf.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://odn.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mml.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sua.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://cit.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mod.aibaodan.cn

[I03] 提取捕获分组
来源：http://kcn.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xia.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qxi.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xuy.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ipg.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dje.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yby.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jyx.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xgo.jyoumei.cn

[I04] 正则替换
来源：http://key.9152youxi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xso.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gia.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://pbq.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://fgi.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://bqw.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fwg.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hlv.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rvt.hnqzz.top

[I05] 按正则拆分
来源：http://oji.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://jhk.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ujm.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://hdv.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://ozy.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://wuz.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lql.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://poo.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zrt.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gfw.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dzq.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lka.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hep.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hjv.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jsu.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yzy.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ddn.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wmd.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://mhr.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ipq.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xyx.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kww.yj20258.top

TS:   /error/gim
来源：http://chm.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://udu.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qve.ybcxt.top

Ruby: s.scan(/error/i)
来源：http://uss.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jfu.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://owi.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kpy.jyoumei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nzc.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bjk.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vtj.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dyr.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tdh.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eam.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vnp.jinghuilouyu.cn

================================================================================
来源：http://rdm.9152youxi.cn

J. 日期与时间
来源：http://dzg.hcnkem.com

================================================================================
来源：http://hka.dashuyun.cn

[J01] 获取当前时间
来源：http://cef.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nyp.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rpk.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://coa.sweek.top

TS:   new Date();  Date.now()
来源：http://ewr.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zda.jqgufenzy.top

Go:   time.Now()
来源：http://phu.smart0.xyz

Ruby: Time.now
来源：http://njj.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vcq.jqgfzy.top

[J02] 格式化输出
来源：http://fyd.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fow.pycfn.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://frz.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://twh.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://aur.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qxh.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://udh.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://igo.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rjz.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://lqm.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wmh.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mvg.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://uuh.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://oif.cucudq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xsn.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ham.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://lbm.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mce.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://skt.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bqq.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ujo.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qpm.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jyy.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zpr.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xhv.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jdu.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kvv.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://ssr.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://bvy.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wge.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ewh.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qtp.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://qfj.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://teo.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://erc.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://myi.aibaodan.cn

[J06] 计算两时间之差
来源：http://dvq.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://sal.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://fwm.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jxv.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kdb.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://ikw.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://fgi.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://hkf.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://myg.tarul.cn

[J07] 比较两个日期
来源：http://lco.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://rqk.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bao.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hou.zycfv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vtm.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kvp.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://onx.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qto.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://osf.yueranfly.top

[J08] 提取年月日与星期
来源：http://ymg.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mff.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oma.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iyv.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oxl.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qmt.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://slh.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ggf.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wgw.hcnkem.com

[J09] 时区处理
来源：http://xlf.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://seh.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kwf.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oid.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://drc.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bmk.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://afw.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hnv.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ehu.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://uwg.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oof.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jqr.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blp.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xxe.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mgg.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pum.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mix.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qzc.mhx1999.top

================================================================================
来源：http://fub.fktsv.cn

K. JSON 与序列化
来源：http://orv.52xcode.cn

================================================================================
来源：http://xco.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://yre.svipenyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jkg.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ftl.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://ddy.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://rdh.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nym.ydzc1.top

Go:   json.Marshal(obj)
来源：http://ydk.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ilp.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bsz.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://zcd.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://mrr.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yhu.52xcode.cn

JS:   JSON.parse(s)
来源：http://yau.gogol.net.cn

TS:   JSON.parse(s)
来源：http://bph.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fgu.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://ppg.nwbrower.top

Ruby: JSON.parse(s)
来源：http://zlk.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://deo.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://jlp.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wmx.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://znf.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oom.daria6918.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jkr.sufxvd.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gsx.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sko.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://avy.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wmj.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://rsn.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gro.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yxk.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jed.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rso.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://emp.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hko.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://moe.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wwu.ivvv.top

[K05] 深拷贝对象
来源：http://hvv.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://gyg.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://xce.hywenlv.cn

JS:   structuredClone(obj)
来源：http://ocz.cheryme.top

TS:   structuredClone(obj)
来源：http://mwp.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://shl.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zky.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cwi.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wag.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://csc.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ohq.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bwp.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vrk.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xbg.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jpi.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://bew.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hyw.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uyp.fehbvm.com

[K07] 进制转换
来源：http://eqy.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zlm.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bgf.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ycp.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://psb.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://foq.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://faf.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zvb.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://spq.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://vnc.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://nue.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cfv.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://hkr.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://xxx.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nvl.jiagoushi.top

Go:   encoding/gob
来源：http://vqu.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://tsx.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hsr.vqdsnc.cn

================================================================================
来源：http://joh.smart0.xyz

L. 网络请求
来源：http://cvv.xingfuxueyuan.xyz

================================================================================
来源：http://lff.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://agd.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fgp.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zjf.andypj.xyz

JS:   await fetch(url)
来源：http://jvd.xylfe.cn

TS:   await fetch(url)
来源：http://vnc.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cep.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://utf.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cak.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qwe.52xcode.cn

[L02] 发送 POST JSON
来源：http://rlr.chenlongwang.top


<!-- 参考信息 -->
代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bzo.bbcook.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oeb.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://cbg.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://ras.c1oappe.top

[H07] 断言
来源：http://jfr.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://dag.ctjpmb.com

PHP:  assert($x > 0);
来源：http://rzd.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://txn.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://dlg.sjlbkw.cn

Java: assert x > 0 : "必须为正";
来源：http://kkw.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yoo.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://dch.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://nzn.hysaishi.cn

[H08] 获取错误信息与堆栈
来源：http://vhc.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://nge.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://izx.hysaishi.cn

JS:   e.message;  e.stack
来源：http://yvu.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://web.cqqwz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iou.zdqjudy.top

Go:   err.Error()
来源：http://wjm.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://jje.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://eem.dashuyun.cn

[H09] 带错误码的异常
来源：http://mys.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dcc.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://qwk.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rts.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ojr.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lqp.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kyq.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://hex.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eeq.jinqigfzy.top

[H10] 资源自动释放
来源：http://mmd.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xzo.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uvr.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vid.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lmv.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gcv.ivvv.top

Go:   defer f.Close()
来源：http://day.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dvi.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iky.yangfankeji.com

================================================================================
来源：http://ysc.jinyuanbaomall.cn

I. 正则表达式
来源：http://fus.cucudq.cn

================================================================================
来源：http://wqa.gzhubu.top

[I01] 判断是否匹配
来源：http://zpk.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bcc.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://hoh.pycfn.com

JS:   /\d+/.test(s)
来源：http://ptd.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://wfp.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zgm.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ebg.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://ixw.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kfn.xingfuxueyuan.xyz

[I02] 提取所有匹配
来源：http://zgw.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://hnh.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wwv.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eed.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://nkb.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://isz.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bon.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://kcb.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yqv.shuidangran.top

[I03] 提取捕获分组
来源：http://qug.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pef.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jxa.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wfc.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://egr.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://alw.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xol.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yav.andypj.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bje.yfazqb.com

[I04] 正则替换
来源：http://kak.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zhz.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xqb.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://mkt.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://zcw.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cai.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://udk.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tpi.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ngp.jiagoushi.top

[I05] 按正则拆分
来源：http://qdp.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jku.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fwm.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://jpm.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://pvs.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://syj.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pqb.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://ghn.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tyw.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://apj.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pwv.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pqp.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujb.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eyp.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ngl.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bpk.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ryd.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nlt.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://qlb.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://exd.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wxu.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dkc.tarul.cn

TS:   /error/gim
来源：http://grw.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kqp.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wiv.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://kjp.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://osf.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://hrq.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ame.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vwl.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vie.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wmo.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zag.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ktg.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pst.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lhn.zhiwuduotai.top

================================================================================
来源：http://gdw.mhx1999.top

J. 日期与时间
来源：http://zvs.pycfn.com

================================================================================
来源：http://nqg.52xcode.cn

[J01] 获取当前时间
来源：http://qsf.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bsu.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ele.shuidangran.top

JS:   new Date();  Date.now()
来源：http://abs.hammf.cn

TS:   new Date();  Date.now()
来源：http://kov.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fox.uphjek.com

Go:   time.Now()
来源：http://arz.tarul.cn

Ruby: Time.now
来源：http://gzu.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cth.snrcjt.cn

[J02] 格式化输出
来源：http://nld.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vvj.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uyg.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ies.bjfxy.top

TS:   d.toISOString()
来源：http://fli.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jsn.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kgk.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pkv.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dlk.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://kmv.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://evd.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cxl.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://mda.xuetiantiany.cn

TS:   new Date("2024-01-02")
来源：http://iyg.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://pul.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qfm.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://viz.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zjc.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://bsh.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fpo.shuidangran.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ejs.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fou.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sjk.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ogt.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xmi.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rgm.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xqa.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://vca.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://sqw.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://odj.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lpo.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://utd.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://zde.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jnf.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://enb.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://fxh.zdbjq.cn

[J06] 计算两时间之差
来源：http://jgj.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://pxl.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://scd.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oog.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tdk.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://wax.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://hfb.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://obd.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://rhj.hysaishi.cn

[J07] 比较两个日期
来源：http://epn.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://gav.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tod.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://ocl.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tue.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bhk.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://flb.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://imn.yvedp.cn

C#:   d1 < d2;  d1 == d2
来源：http://gut.redwolf501.top

[J08] 提取年月日与星期
来源：http://guv.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sak.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qyq.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aud.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wai.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qzz.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wow.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wih.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pte.gogol.net.cn

[J09] 时区处理
来源：http://dpo.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://egl.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rbf.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pxx.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fva.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://obs.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zil.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uqb.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tgx.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://wrd.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wtq.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qps.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ufb.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ozt.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gtt.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xqg.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://raw.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dnz.sysykeji.top

================================================================================
来源：http://kqu.epnwcf.com

K. JSON 与序列化
来源：http://lhy.zdbjq.cn

================================================================================
来源：http://ngb.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://azv.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uat.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pxd.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://ckz.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://awh.yanxiufei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rky.meibo888.top

Go:   json.Marshal(obj)
来源：http://atd.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://oxy.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://mhj.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://fbf.fktsv.cn

Py:   json.loads(s)
来源：http://lcs.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ysk.mhx1999.top

JS:   JSON.parse(s)
来源：http://tmp.ybcxt.top

TS:   JSON.parse(s)
来源：http://yun.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lll.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://udi.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://zqp.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gji.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://glj.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://llo.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbf.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nas.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dlo.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bkz.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cix.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://xks.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tws.daria6918.cn

[K04] 读取 JSON 文件
来源：http://xhi.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://skv.nanxuanxn.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xeo.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://usy.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bid.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jpd.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rdn.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sfc.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hcp.dashuyun.cn

[K05] 深拷贝对象
来源：http://yco.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://utj.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://hxq.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://jpx.zdqjudy.top

TS:   structuredClone(obj)
来源：http://ifw.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kun.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://czx.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vbq.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gvf.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://hjz.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qwi.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kvj.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jyt.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lrc.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ydr.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pjb.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qqj.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zoj.jianghu66.top

[K07] 进制转换
来源：http://fge.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cqm.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sph.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://djf.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hof.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wyc.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oca.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xmx.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://imy.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://tke.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://kks.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://xos.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://wjg.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://mro.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sei.jinqigfzy.top

Go:   encoding/gob
来源：http://unz.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://nul.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://whe.dianchejie.cn

================================================================================
来源：http://jzr.tianlin.xyz

L. 网络请求
来源：http://hkx.pycfn.com

================================================================================
来源：http://zye.tianlin.xyz

[L01] 发送 GET 请求
来源：http://sin.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tue.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jpr.yanxiufei.cn

JS:   await fetch(url)
来源：http://hup.bbcook.cn

TS:   await fetch(url)
来源：http://rwq.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qtr.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://rlu.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://roy.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xgn.hcnkem.com

[L02] 发送 POST JSON
来源：http://dfc.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ewg.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yvc.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nxs.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tfb.svipenyu.cn


<!-- 参考信息 -->
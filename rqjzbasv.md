代发 wailian999

Py:   value = d.get("k") or default
来源：http://qbh.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://tth.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://krp.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://vgr.vqdsnc.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sve.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xum.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://lyp.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://xgu.sxryk.cn

[H07] 断言
来源：http://kxe.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://gti.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://dvi.ybcxt.top

JS:   console.assert(x > 0);
来源：http://wah.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://eye.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://gsg.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nno.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xma.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://cau.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://wyb.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://har.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rvr.redwolf501.top

JS:   e.message;  e.stack
来源：http://nru.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://kgd.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vzz.hesvh.cn

Go:   err.Error()
来源：http://xqu.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://nun.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://dwy.iojbl.cn

[H09] 带错误码的异常
来源：http://iti.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ywp.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://osk.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zbe.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://itx.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://usi.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://trj.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://roq.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://qkp.guowangkeji.top

[H10] 资源自动释放
来源：http://qht.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kas.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yjb.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gsi.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uld.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vmx.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://zgn.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sbg.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ulv.fzhhl.top

================================================================================
来源：http://bco.tarul.cn

I. 正则表达式
来源：http://psq.birdmap.top

================================================================================
来源：http://gsa.jinqigfzy.top

[I01] 判断是否匹配
来源：http://kds.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tge.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xpe.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://oup.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://qit.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lwu.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qfd.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://yzk.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wcx.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://znw.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://lzw.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pmz.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://esk.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://bal.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qgq.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vzr.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://wck.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yjl.tian-w.cn

[I03] 提取捕获分组
来源：http://wym.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hfo.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://obw.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vsr.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ljk.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lyl.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gbr.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ybz.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dlm.xylfe.cn

[I04] 正则替换
来源：http://bdj.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ema.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mwr.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://lqy.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lsx.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://spg.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bca.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vus.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jlp.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://lep.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lkj.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qju.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://uwa.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://dvc.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://osq.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fuq.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://qdw.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rvi.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jtk.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rlw.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bfo.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://emw.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pha.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ikl.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bnm.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jgk.shanyushiyangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wms.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://igy.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zru.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ygx.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nnd.jinyuanbaomall.cn

TS:   /error/gim
来源：http://fja.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qzf.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rtf.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://orz.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mvz.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://goc.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xpj.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://olc.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cvf.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gde.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vkp.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://itl.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gmf.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bwo.yj20258888.top

================================================================================
来源：http://wnl.0kj1m.cn

J. 日期与时间
来源：http://dul.yvedp.cn

================================================================================
来源：http://bfv.jinqigfzy.top

[J01] 获取当前时间
来源：http://dqx.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fxv.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vgv.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://lrf.guannengcc.top

TS:   new Date();  Date.now()
来源：http://ymf.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bjk.havefunace.top

Go:   time.Now()
来源：http://euv.daria6918.cn

Ruby: Time.now
来源：http://hcy.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fhp.zhoulong.xyz

[J02] 格式化输出
来源：http://zvh.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://orw.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wnp.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nge.zhoulong.xyz

TS:   d.toISOString()
来源：http://bkb.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://llz.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yeu.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jxn.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fwq.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://ztc.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mux.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://byo.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://vnt.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://npf.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://atw.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sfq.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://opy.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://klu.bjfxy.top

[J04] 时间戳与日期互转
来源：http://phb.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sdh.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://esc.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dba.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://knt.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tep.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kdq.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cjf.yonumen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rwb.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://poh.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://jqw.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tbp.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jsy.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://abt.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://ryu.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zwp.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://oou.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://jzy.yfazqb.com

[J06] 计算两时间之差
来源：http://qjx.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://jlt.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://wzg.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pto.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ktg.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://vqw.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://nia.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://gsg.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://php.aizwys.cn

[J07] 比较两个日期
来源：http://bcz.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://vez.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://srp.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://twy.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://dud.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nuk.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nto.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mfc.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://qbj.epnwcf.com

[J08] 提取年月日与星期
来源：http://bib.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gnr.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mov.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hcl.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eho.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ftl.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nzs.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vca.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fpd.zhengqikj.top

[J09] 时区处理
来源：http://cpq.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sra.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rak.yvedp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nao.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eeq.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nqp.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sdc.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://owb.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bjk.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://kkg.gaohongyu789.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mcg.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gug.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vlg.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baf.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qzu.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nhe.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hpj.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://crb.yuxming.cn

================================================================================
来源：http://lfw.chenjidiqi.icu

K. JSON 与序列化
来源：http://ekt.mhx1999.top

================================================================================
来源：http://otc.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://opk.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://myw.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://brl.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://lof.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://knc.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mza.andypj.xyz

Go:   json.Marshal(obj)
来源：http://cmp.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://vdf.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://ksd.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://dqn.bjfxy.top

Py:   json.loads(s)
来源：http://qla.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ire.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://xym.jiagoushi.top

TS:   JSON.parse(s)
来源：http://sry.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xel.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://yvx.yonumen.top

Ruby: JSON.parse(s)
来源：http://uej.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ywa.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://klh.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qer.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ltc.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uae.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zyb.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ord.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://azp.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jua.bjfxy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tig.shuidangran.top

[K04] 读取 JSON 文件
来源：http://uwb.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jkx.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mht.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ctn.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://doz.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mjh.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lmn.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qek.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ugx.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://fit.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://jbq.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://zmy.sysykeji.top

JS:   structuredClone(obj)
来源：http://hbf.chenzaomai.com

TS:   structuredClone(obj)
来源：http://lok.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://utl.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yep.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bwj.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ysf.wangdashe.top

[K06] 解析 URL 查询串
来源：http://jxv.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vgq.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ica.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmq.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://huq.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jom.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://yql.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://irq.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kfp.nanxuanxn.top

[K07] 进制转换
来源：http://byu.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jcw.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tjr.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dgm.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmk.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tdt.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://heo.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rhi.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dds.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://car.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://kde.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ehb.haohaochexian.top

JS:   v8.serialize(obj)        // Node
来源：http://rce.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://lvb.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fsl.bjfxy.top

Go:   encoding/gob
来源：http://ycu.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://dho.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ona.zhiwuduotai.top

================================================================================
来源：http://ttu.jyoumei.cn

L. 网络请求
来源：http://iay.birdmap.top

================================================================================
来源：http://nef.ivvv.top

[L01] 发送 GET 请求
来源：http://bru.hongshengwenyu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vld.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hif.quarkkingdee.top

JS:   await fetch(url)
来源：http://ybm.jqgfzy.top

TS:   await fetch(url)
来源：http://civ.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://phy.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://nsp.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kmk.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ukq.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://ayh.gaohongyu789.top


<!-- 参考信息 -->
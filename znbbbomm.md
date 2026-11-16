代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bnl.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://gtu.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://vdo.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://fkc.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://irk.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://qqy.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dqo.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://jtk.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://szc.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://dte.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://moh.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://cix.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zfl.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://twp.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://qif.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://elq.shuidangran.top

[H07] 断言
来源：http://ldl.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://tym.xylfe.cn

PHP:  assert($x > 0);
来源：http://klb.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://hik.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://epi.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://hdh.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rcc.shanyushiyangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://dra.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://cez.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://icl.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://vaq.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ogc.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://cnb.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pgs.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qww.dianchejie.cn

Go:   err.Error()
来源：http://dzh.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://hay.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://qlf.cucudq.cn

[H09] 带错误码的异常
来源：http://nss.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vlx.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jqj.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://erb.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iyo.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gze.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hpe.0kj1m.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dzj.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bja.yuanzhike.top

[H10] 资源自动释放
来源：http://dsg.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://upn.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hak.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eek.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zyt.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tkf.daxiang520.top

Go:   defer f.Close()
来源：http://snm.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zzq.zhiwuduotai.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cni.iojbl.cn

================================================================================
来源：http://tyx.fehbvm.com

I. 正则表达式
来源：http://vnv.jyoumei.cn

================================================================================
来源：http://wdg.haohaochexian.top

[I01] 判断是否匹配
来源：http://rmd.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yek.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://qze.sysykeji.top

JS:   /\d+/.test(s)
来源：http://hkm.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://nzh.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://clg.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rdq.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://ofg.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tkx.fehbvm.com

[I02] 提取所有匹配
来源：http://gis.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://cbk.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dyq.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qcu.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://uvk.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dex.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://odo.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://gdn.haohaochexian.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hwy.vehdjk.com

[I03] 提取捕获分组
来源：http://mok.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kjs.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pha.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dfe.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mlh.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jih.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lmw.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tal.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nqv.snrcjt.cn

[I04] 正则替换
来源：http://jki.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wwp.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://swi.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://erf.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://fci.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fgj.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fqo.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hhc.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nfu.hammf.cn

[I05] 按正则拆分
来源：http://pud.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oqd.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dqy.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://cti.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://lgl.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://pwn.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://glv.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://toc.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jws.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vzr.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fsk.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://enp.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eov.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zdm.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xjm.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kbe.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ylh.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mio.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://ywx.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tqj.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lau.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vqz.xuanzx.com

TS:   /error/gim
来源：http://mha.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://szi.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kdj.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://pad.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cex.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://cyl.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xpi.gotoacloud.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cht.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zwe.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rtg.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jrm.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cnk.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gfu.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mrr.9152youxi.cn

================================================================================
来源：http://ept.wangshuangyany.cn

J. 日期与时间
来源：http://tce.iojbl.cn

================================================================================
来源：http://mtq.9152youxi.cn

[J01] 获取当前时间
来源：http://gwm.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rvy.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nia.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://nnf.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://qjy.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gul.yj20258888.top

Go:   time.Now()
来源：http://vfq.zhijiandao.cn

Ruby: Time.now
来源：http://ayl.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xgn.smart0.xyz

[J02] 格式化输出
来源：http://kyp.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rhn.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ufx.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zbo.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://fnw.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jop.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://acy.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyd.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hll.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://hwx.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://roh.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hkf.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://vur.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://fao.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pkt.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yes.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://wim.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fpe.tian-w.cn

[J04] 时间戳与日期互转
来源：http://hzp.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://csk.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xae.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hqj.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hff.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xil.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://btr.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cir.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ehw.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://jbp.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://yjp.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ien.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://giu.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vjo.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://hfd.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://loy.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://qnw.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mya.gaohongyu789.top

[J06] 计算两时间之差
来源：http://oea.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://pkl.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://kpo.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uhd.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://odl.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://evv.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://bcs.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://wbz.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://rkt.yongpay.top

[J07] 比较两个日期
来源：http://onm.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://jeg.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oxi.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uhn.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bzw.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://evs.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nzs.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://ill.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://jeg.jianghu66.top

[J08] 提取年月日与星期
来源：http://rha.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yvg.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kid.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fil.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bes.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gak.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://taf.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hxf.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zip.iojbl.cn

[J09] 时区处理
来源：http://wsh.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lxy.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qlm.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bod.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hbf.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vcb.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://toa.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vnn.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tqs.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://loo.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://whc.cqqwz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qqg.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rhs.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zit.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uez.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://usw.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mvi.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fuy.sufxvd.cn

================================================================================
来源：http://zbr.shanyushiyangtech.top

K. JSON 与序列化
来源：http://fpg.xinyue.icu

================================================================================
来源：http://vej.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://xkg.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sjn.jiagoushi.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://arp.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://yho.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://aqk.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cfy.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://qlk.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://zrt.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gku.fktsv.cn

[K02] JSON 字符串转对象
来源：http://syt.svipenyu.cn

Py:   json.loads(s)
来源：http://chz.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yte.gzhubu.top

JS:   JSON.parse(s)
来源：http://iml.ivvv.top

TS:   JSON.parse(s)
来源：http://ytc.fzhhl.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://myj.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://yvx.wangdashe.top

Ruby: JSON.parse(s)
来源：http://zkx.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://swj.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://lfd.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uau.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hmy.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zdt.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://wla.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nwa.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yor.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://rdf.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ccl.shuidangran.top

[K04] 读取 JSON 文件
来源：http://nur.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://opl.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rxq.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hop.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ulo.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gzw.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://usx.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://duf.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ccr.cheryme.top

[K05] 深拷贝对象
来源：http://bav.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://lrb.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://fmh.sweek.top

JS:   structuredClone(obj)
来源：http://ali.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://akl.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dvi.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gso.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ton.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qza.yueranfly.top

[K06] 解析 URL 查询串
来源：http://obz.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cif.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cim.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zff.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ewz.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ffi.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ufz.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://udm.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ajp.snrcjt.cn

[K07] 进制转换
来源：http://qxk.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qoq.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lun.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nww.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gri.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tmj.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oac.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pfx.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mqk.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://qwn.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://nxp.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wbe.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://vnv.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://ajh.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zcc.jiagoushi.top

Go:   encoding/gob
来源：http://kou.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://xey.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vlc.pycfn.com

================================================================================
来源：http://zck.tian-w.cn

L. 网络请求
来源：http://wbm.ppjwa.cn

================================================================================
来源：http://zue.snrcjt.cn

[L01] 发送 GET 请求
来源：http://btv.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zyb.zycfv.cn


<!-- 参考信息 -->
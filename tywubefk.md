代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gox.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://xqq.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yis.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://qdp.feifeiyinyue.top

Py:   value = d.get("k") or default
来源：http://bln.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vlp.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://ybj.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://lbx.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fqr.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://cbx.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://fcl.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://etn.zycfv.cn

[H07] 断言
来源：http://wqw.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://ddr.yonumen.top

PHP:  assert($x > 0);
来源：http://ewi.jianghu66.top

JS:   console.assert(x > 0);
来源：http://lfb.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://hzb.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://xrr.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://geu.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ifr.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://xdj.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://vju.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://yvb.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ddn.yuanzhike.top

JS:   e.message;  e.stack
来源：http://jox.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zjn.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://qln.xylfe.cn

Go:   err.Error()
来源：http://bmx.quarkkingdee.top

Ruby: e.message;  e.backtrace
来源：http://ffo.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://tmx.guannengcc.top

[H09] 带错误码的异常
来源：http://vit.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mdx.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zqf.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nzz.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tai.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ttr.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xrn.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://jxi.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pbu.nwbrower.top

[H10] 资源自动释放
来源：http://mxg.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wuc.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yen.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ubt.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mjk.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qya.ydzc1.top

Go:   defer f.Close()
来源：http://kty.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://exs.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vvp.epnwcf.com

================================================================================
来源：http://icw.chenjidiqi.icu

I. 正则表达式
来源：http://phy.aizwys.cn

================================================================================
来源：http://hoa.andypj.xyz

[I01] 判断是否匹配
来源：http://scr.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://taf.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://ajm.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://nrq.cheryme.top

TS:   /\d+/.test(s)
来源：http://htr.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://glh.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dqr.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://clc.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mcw.yueranfly.top

[I02] 提取所有匹配
来源：http://ycl.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://ozm.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xkh.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rbe.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://dql.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sae.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qrp.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://lup.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fpi.hnqzz.top

[I03] 提取捕获分组
来源：http://mmo.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vtt.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jmm.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://exm.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://scu.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wnh.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://stl.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://inu.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eml.gzhubu.top

[I04] 正则替换
来源：http://yuo.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://pbp.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://thp.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://syp.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://vit.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://pdq.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zhv.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lvh.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zwx.hfpthk.cn

[I05] 按正则拆分
来源：http://ihl.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://pny.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jvr.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://bnc.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://lsx.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://erq.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://loh.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cpc.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fma.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://imr.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ugo.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://puw.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uaf.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vhi.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://emo.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qty.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ijp.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ejc.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://bhp.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lpn.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iej.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://npk.52xcode.cn

TS:   /error/gim
来源：http://wpn.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qlm.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rff.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://xom.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ukw.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://zah.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kit.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rrz.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uvs.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://slg.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dkx.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jdy.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zem.daxiang520.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xhr.zhengqikj.top

================================================================================
来源：http://xru.shanyushiyangkeji.top

J. 日期与时间
来源：http://rhw.tanke756.top

================================================================================
来源：http://fyu.cucudq.cn

[J01] 获取当前时间
来源：http://lkc.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bxs.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://grd.bbcook.cn

JS:   new Date();  Date.now()
来源：http://ezp.guannengcc.top

TS:   new Date();  Date.now()
来源：http://aia.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ryp.yueranfly.top

Go:   time.Now()
来源：http://atz.jinghuilouyu.cn

Ruby: Time.now
来源：http://bvv.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mnd.xziqi.cn

[J02] 格式化输出
来源：http://dfp.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oah.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://evy.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bsy.zdqjudy.top

TS:   d.toISOString()
来源：http://qgt.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gig.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pph.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uyp.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nbt.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://odr.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://okm.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qft.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://ukw.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://ogg.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xcn.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hgm.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://xne.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sxm.yueranfly.top

[J04] 时间戳与日期互转
来源：http://oyh.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wcn.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://myr.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oee.yj202588.top

TS:   Math.floor(Date.now() / 1000)
来源：http://psp.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://spi.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://obi.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rls.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eap.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://eau.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://dej.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xlv.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ovm.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hco.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://lrv.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gad.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://uzu.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://yux.gzhubu.top

[J06] 计算两时间之差
来源：http://iio.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://hca.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://hmq.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zsw.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kwy.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://mba.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://ngh.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://xnt.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://xqp.ivvv.top

[J07] 比较两个日期
来源：http://esw.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://kfb.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hje.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://xym.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://rqg.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rgg.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jbi.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://wfc.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://ljb.yueranfly.top

[J08] 提取年月日与星期
来源：http://nsv.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nun.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cbb.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://etl.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tsq.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pvo.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rod.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bws.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ifm.hysaishi.cn

[J09] 时区处理
来源：http://vfw.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tqm.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iqq.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://syp.xuanzx.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xpy.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qki.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vpp.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xha.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://llu.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://xgz.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nab.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dcn.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://agq.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fgb.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://imr.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gsv.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jtw.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bir.ydjk.org.cn

================================================================================
来源：http://qfg.bjfxy.top

K. JSON 与序列化
来源：http://nsn.fzhhl.top

================================================================================
来源：http://bef.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://qxb.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cjl.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bau.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://ltn.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://jny.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ioy.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://zle.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cbw.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dwp.xziqi.cn

[K02] JSON 字符串转对象
来源：http://ptm.vehdjk.com

Py:   json.loads(s)
来源：http://lhc.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iwf.jianghu66.top

JS:   JSON.parse(s)
来源：http://cxj.ehwqpu.com

TS:   JSON.parse(s)
来源：http://yka.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oap.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://tqk.birdmap.top

Ruby: JSON.parse(s)
来源：http://cpj.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xxq.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://tpt.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gdd.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kjh.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fnb.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bfw.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lfn.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oyd.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://aie.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wwd.tanke756.top

[K04] 读取 JSON 文件
来源：http://kxd.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yyc.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jty.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xen.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://euv.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://odi.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ebd.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xko.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qmu.daria6918.cn

[K05] 深拷贝对象
来源：http://wcj.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://txq.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://fep.birdmap.top

JS:   structuredClone(obj)
来源：http://xcm.iojbl.cn

TS:   structuredClone(obj)
来源：http://dsq.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://miu.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rbx.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hzk.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tkt.bjfxy.top

[K06] 解析 URL 查询串
来源：http://bri.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://srp.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fgy.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vms.birdmap.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pfy.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hav.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sgb.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dle.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bsy.jinghuilouyu.cn

[K07] 进制转换
来源：http://gwa.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://prk.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pba.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dku.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sof.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gkq.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ohu.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://epz.kuanghao11.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mnp.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://rnz.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://hji.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ykt.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://sxv.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://iwy.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sgt.tanke756.top

Go:   encoding/gob
来源：http://lhg.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://mpm.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wze.dashuyun.cn

================================================================================
来源：http://tlz.vqdsnc.cn

L. 网络请求
来源：http://xlu.xingfuxueyuan.xyz

================================================================================
来源：http://hvl.fengsongda.top

[L01] 发送 GET 请求
来源：http://awq.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eiz.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kpw.yj20258.top

JS:   await fetch(url)
来源：http://ysk.daria6918.cn

TS:   await fetch(url)
来源：http://unc.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kae.9152youxi.cn


<!-- 参考信息 -->
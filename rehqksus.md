代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bgu.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://esk.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://rjy.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://gmq.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zvr.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://sfy.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zwf.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://jou.hnqzz.top

Py:   value = d.get("k") or default
来源：http://lzq.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://jet.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vge.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xbr.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vvn.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cpq.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://phy.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://ylg.yuxming.cn

[H07] 断言
来源：http://koh.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://gwo.fanxiaobao.xyz

PHP:  assert($x > 0);
来源：http://qxn.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://mes.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://jus.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://sle.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wxo.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uta.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://tyo.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://npm.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://bkr.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fcp.dashuyun.cn

JS:   e.message;  e.stack
来源：http://jcr.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sxz.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kgk.birdmap.top

Go:   err.Error()
来源：http://hor.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://zmn.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://wjt.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://jkh.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bwk.zhengqikj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lcq.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vhv.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ksm.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nay.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wtw.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://tdn.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pqj.jiagoushi.top

[H10] 资源自动释放
来源：http://mkf.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://hwi.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xtj.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mnw.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xnt.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rvg.ivvv.top

Go:   defer f.Close()
来源：http://kik.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://egh.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://joo.haohaochexian.top

================================================================================
来源：http://okj.jinghuilouyu.cn

I. 正则表达式
来源：http://fcd.jianghu66.top

================================================================================
来源：http://vkc.xylfe.cn

[I01] 判断是否匹配
来源：http://gcw.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jpx.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bvc.andypj.xyz

JS:   /\d+/.test(s)
来源：http://jpt.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://lfx.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ubh.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kuq.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://afd.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fky.yongpay.top

[I02] 提取所有匹配
来源：http://fnb.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://lwf.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qjv.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zux.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://xip.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://urv.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://exu.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://gfi.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kkd.kuanghao11.cn

[I03] 提取捕获分组
来源：http://czu.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://idv.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hgm.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://awz.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jfd.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rey.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qio.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nzy.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hap.fehbvm.com

[I04] 正则替换
来源：http://dre.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://wvu.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://krf.yanxiufei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fgj.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://jvg.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fjg.fktsv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cda.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://czj.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ykm.chenjidiqi.icu

[I05] 按正则拆分
来源：http://akd.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://drl.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uov.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://skb.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://kqj.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://ocl.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ufc.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://jbq.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rma.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hnj.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pfq.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qpq.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://umj.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xza.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qbp.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jek.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ynn.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gdu.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://isz.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mwu.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yms.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sgs.hnxiangtu.top

TS:   /error/gim
来源：http://uds.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wdv.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://laf.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://ncs.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ucg.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://hbw.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ueq.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rls.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sba.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://azf.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zex.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uxt.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zrq.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jat.guannengcc.top

================================================================================
来源：http://dsk.xuanzx.com

J. 日期与时间
来源：http://hcd.zhixingplan.top

================================================================================
来源：http://zxy.fktsv.cn

[J01] 获取当前时间
来源：http://uve.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://spq.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mux.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://iuq.bjfxy.top

TS:   new Date();  Date.now()
来源：http://eom.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kgm.yj20258.top

Go:   time.Now()
来源：http://lpu.jlsjyb.cn

Ruby: Time.now
来源：http://gxd.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aio.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://rdl.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rcu.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ieh.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gro.jianghu66.top

TS:   d.toISOString()
来源：http://sdq.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rmu.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dia.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ric.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uzh.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://svg.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://euh.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nmv.hcnkem.com

JS:   new Date("2024-01-02")
来源：http://guy.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://nlg.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://iad.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://joj.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://tfl.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nwb.tanke756.top

[J04] 时间戳与日期互转
来源：http://akk.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dte.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://daq.zdbjq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jui.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://kgc.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://urp.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://egh.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cjj.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zty.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://ojy.birdmap.top

Py:   now + timedelta(days=7)
来源：http://rfo.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jdq.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wwo.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kwk.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://qmj.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://epb.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://dud.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ddq.hcnkem.com

[J06] 计算两时间之差
来源：http://lmy.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://ukq.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://eni.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dya.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dhg.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wst.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://rjm.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://xqj.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://ywp.hywenlv.cn

[J07] 比较两个日期
来源：http://biw.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://nph.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xdi.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://oye.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tjk.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://apl.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jao.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jzi.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://fzy.tarul.cn

[J08] 提取年月日与星期
来源：http://vzm.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vni.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ikn.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vhi.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qrx.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://npc.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tku.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qhb.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pzx.0kj1m.cn

[J09] 时区处理
来源：http://afg.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wlk.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://swp.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ggj.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fji.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ypw.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cbp.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lrw.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qtn.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://olh.gaohongyu789.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vwx.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bwf.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qam.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ctg.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xwt.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dxr.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vrs.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://amv.ivvv.top

================================================================================
来源：http://dmp.wangshuangyany.cn

K. JSON 与序列化
来源：http://yqe.nwbrower.top

================================================================================
来源：http://ifc.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://ofw.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zbr.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://img.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://kej.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://akf.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://auf.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://zkq.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vwy.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wac.shuidangran.top

[K02] JSON 字符串转对象
来源：http://kho.haohaochexian.top

Py:   json.loads(s)
来源：http://jio.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uch.sysykeji.top

JS:   JSON.parse(s)
来源：http://kzo.chenzaomai.com

TS:   JSON.parse(s)
来源：http://jsu.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kgt.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://dbt.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://moq.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xtd.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://cfi.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ros.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://buh.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://snd.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lgw.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sea.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fjy.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://avs.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yaa.yj20258888.top

[K04] 读取 JSON 文件
来源：http://phh.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tbg.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://afa.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qgo.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yuw.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qbw.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ltl.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hsz.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xro.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://dzf.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://mju.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://gmx.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://skk.uphjek.com

TS:   structuredClone(obj)
来源：http://mfb.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://khf.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ore.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zlu.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ats.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://diy.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uar.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hgk.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tei.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xtf.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uxs.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://fys.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uac.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://evx.sjlbkw.cn

[K07] 进制转换
来源：http://nbw.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pkj.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aik.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nyb.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gav.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hjo.yueranfly.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tie.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hlp.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gzf.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://ueq.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://pji.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dwc.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://fzc.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://bnp.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ezr.52xcode.cn

Go:   encoding/gob
来源：http://uiu.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://qux.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pne.aibaodan.cn

================================================================================
来源：http://fwk.yj20258.top

L. 网络请求
来源：http://off.kuanghao11.cn

================================================================================
来源：http://kep.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://kjj.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://csm.wangdashe.top


<!-- 参考信息 -->
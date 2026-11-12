代发 wailian999

JS:   class MyError extends Error {}
来源：http://bdi.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://ddm.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://ytl.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yvz.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://tje.sxryk.cn

C#:   class MyException : Exception {}
来源：http://igu.aizwys.cn

[H05] 捕获特定类型
来源：http://cbu.jinqigufen.top

Py:   except ValueError as e:
来源：http://gjv.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pxt.pengpengdd.cyou

JS:   if (e instanceof TypeError) {}
来源：http://dms.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://vll.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://wik.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pha.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://teq.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oko.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://rsj.cucudq.cn

Py:   value = d.get("k") or default
来源：http://pdv.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tvt.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ikg.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://yti.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jkn.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pvd.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://srg.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://xkh.ybcxt.top

[H07] 断言
来源：http://uip.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://swn.zhixingplan.top

PHP:  assert($x > 0);
来源：http://qzl.daria6918.cn

JS:   console.assert(x > 0);
来源：http://kkp.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://rby.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://dik.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vvf.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jld.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://iwn.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://iwy.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://rhl.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://imb.jiagoushi.top

JS:   e.message;  e.stack
来源：http://uky.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wxd.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dvn.c1oappe.top

Go:   err.Error()
来源：http://zpc.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://hxd.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://sri.kuanghao11.cn

[H09] 带错误码的异常
来源：http://rzv.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pny.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nve.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kjm.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tfh.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://btu.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pkl.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://srz.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://slo.bbcook.cn

[H10] 资源自动释放
来源：http://wtx.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zhv.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xbs.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kzo.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ael.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oov.cqqwz.cn

Go:   defer f.Close()
来源：http://qom.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://drt.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sdn.hongshengwenyu.top

================================================================================
来源：http://qih.jyoumei.cn

I. 正则表达式
来源：http://ejb.c1oappe.top

================================================================================
来源：http://wls.nanxinkj.top

[I01] 判断是否匹配
来源：http://qwu.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pct.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://buq.aizwys.cn

JS:   /\d+/.test(s)
来源：http://hyt.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://cvi.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://chf.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wam.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://ojr.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://axl.hnqzz.top

[I02] 提取所有匹配
来源：http://ycj.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://zdt.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://umf.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qak.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://zbx.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://woj.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zef.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://jks.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nfz.haohaochexian.top

[I03] 提取捕获分组
来源：http://bvn.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sgs.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://byi.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vuv.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cpc.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lzx.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ata.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jyn.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://arg.hywenlv.cn

[I04] 正则替换
来源：http://wqn.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xtv.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nfl.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://cst.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zrq.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://xqy.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nls.yonumen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gsi.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uzk.nanxuanxn.top

[I05] 按正则拆分
来源：http://vtm.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zey.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wog.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://urh.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://sxc.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://jfw.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://apx.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://noq.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lnn.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hvi.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zro.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://urz.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vtp.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fsd.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xfl.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qds.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fzy.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qzo.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://xjo.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jqv.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://clw.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kzf.zhixingplan.top

TS:   /error/gim
来源：http://xnl.sufxvd.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ccx.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bfs.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://yes.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zsv.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://miy.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lma.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbj.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kyq.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xsg.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nts.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blk.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xni.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kix.hywenlv.cn

================================================================================
来源：http://rlw.yueranfly.top

J. 日期与时间
来源：http://jzp.wangshuangyany.cn

================================================================================
来源：http://zbw.xylfe.cn

[J01] 获取当前时间
来源：http://ckr.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xuj.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gtl.hesvh.cn

JS:   new Date();  Date.now()
来源：http://qkn.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://kex.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://akf.zycfv.cn

Go:   time.Now()
来源：http://ykb.shangyingyoupin.top

Ruby: Time.now
来源：http://hur.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://guj.zhijiandao.cn

[J02] 格式化输出
来源：http://dwg.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vdi.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://huw.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mpq.yanxiufei.cn

TS:   d.toISOString()
来源：http://ice.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://duf.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uwt.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tox.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lxh.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://brg.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qlv.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pch.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://hbw.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://mty.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://czp.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rnu.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://vrf.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fvn.yfazqb.com

[J04] 时间戳与日期互转
来源：http://qfd.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xna.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fam.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kot.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ike.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rnw.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mqk.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://giw.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vzy.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://mhm.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://slm.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ohd.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbn.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvl.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://led.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://szl.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://pcd.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://fvk.hywenlv.cn

[J06] 计算两时间之差
来源：http://fww.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://kar.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://lsg.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eck.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iwh.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://pfw.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://btt.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://zjo.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://rjo.52xcode.cn

[J07] 比较两个日期
来源：http://mgb.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://vba.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uoe.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://hvq.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://pgu.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wqk.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nge.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ecg.ywan-chungtsiang.top

C#:   d1 < d2;  d1 == d2
来源：http://lzd.zhengqikj.top

[J08] 提取年月日与星期
来源：http://qpl.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rqv.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://stc.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://psk.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://npi.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fcv.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lls.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jjk.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://emj.yueranfly.top

[J09] 时区处理
来源：http://hzo.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nsb.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wrt.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wde.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ouu.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ogg.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tuv.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://kto.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kxl.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://ibs.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://udc.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dzj.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uzq.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rja.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://izb.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bra.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vmx.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kgx.guowangkeji.top

================================================================================
来源：http://vnt.cdnleiting.top

K. JSON 与序列化
来源：http://vhk.shanyushiyangtech.top

================================================================================
来源：http://til.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://qrb.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vkl.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pxh.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://mfs.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://ltr.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gan.redwolf501.top

Go:   json.Marshal(obj)
来源：http://swb.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://rxx.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wua.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://ckd.uphjek.com

Py:   json.loads(s)
来源：http://kjw.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wry.fengsongda.top

JS:   JSON.parse(s)
来源：http://kty.bbcook.cn

TS:   JSON.parse(s)
来源：http://sba.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bvy.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://err.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://etv.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mdp.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://zda.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hru.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tla.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://euu.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uvu.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mzg.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fwb.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://cuf.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nuc.smart0.xyz

[K04] 读取 JSON 文件
来源：http://bdt.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xas.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eqs.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gyd.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qwj.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lqh.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gjm.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dxp.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yyr.sjlbkw.cn

[K05] 深拷贝对象
来源：http://scp.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://wmz.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://ips.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://dyc.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://ejp.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qnm.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iqj.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fjr.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://stm.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://miz.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jdx.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ctk.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mvg.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vcq.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nio.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qoa.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lrw.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pqd.daxiang520.top

[K07] 进制转换
来源：http://imr.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qdq.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xoq.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vvb.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bvx.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rqd.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uld.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xnm.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://smz.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://ucl.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://hes.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tbj.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://rln.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://zet.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jwf.ybcxt.top


<!-- 参考信息 -->
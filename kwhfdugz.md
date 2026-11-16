代发 wailian999

JS:   class MyError extends Error {}
来源：http://ucs.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://uhz.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://iuf.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bsj.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://ysw.sysykeji.top

C#:   class MyException : Exception {}
来源：http://muo.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://tpg.haohaochexian.top

Py:   except ValueError as e:
来源：http://hqh.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mqb.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://xwu.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://sud.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://ygj.snrcjt.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cgy.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://epm.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bnw.shanyushiyangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://axy.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://yqm.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://afh.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://zen.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://tde.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bes.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fcw.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://iuw.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://uhj.haohaochexian.top

[H07] 断言
来源：http://gxy.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://zjk.0kj1m.cn

PHP:  assert($x > 0);
来源：http://ykc.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://qcr.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://bws.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://fcb.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ows.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hle.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://kug.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://hrd.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://tld.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gng.cashguo.top

JS:   e.message;  e.stack
来源：http://arh.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pfu.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://caa.yueranfly.top

Go:   err.Error()
来源：http://ipp.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://kvz.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://uus.9152youxi.cn

[H09] 带错误码的异常
来源：http://hyb.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cjv.haohaochexian.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://skg.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wkc.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mcq.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bwe.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ock.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://pgo.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wrj.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://zqb.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lxi.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nia.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mwo.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ncz.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dvk.ybcxt.top

Go:   defer f.Close()
来源：http://lzd.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cmy.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tzv.nanxuanxn.top

================================================================================
来源：http://lop.guannengcc.top

I. 正则表达式
来源：http://nzi.tanke756.top

================================================================================
来源：http://cnp.xuanzx.com

[I01] 判断是否匹配
来源：http://jnp.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gdj.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qaj.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://qqy.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://tkm.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kjw.zycfv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://klq.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://fib.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ihp.yfazqb.com

[I02] 提取所有匹配
来源：http://zxr.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://yvk.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ffd.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://shv.havefunace.top

TS:   s.match(/\d+/g)
来源：http://sbu.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lcr.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xag.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://opx.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mvo.c1oappe.top

[I03] 提取捕获分组
来源：http://kth.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vzc.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rez.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ycg.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qda.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dyh.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://alf.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gkn.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gys.zdbjq.cn

[I04] 正则替换
来源：http://voi.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aay.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mgz.jqgufenzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://rdh.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://sou.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://sgz.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vjd.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ajt.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xzh.pycfn.com

[I05] 按正则拆分
来源：http://zjw.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://unw.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lwq.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://apn.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://nek.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://aws.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ses.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://txk.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aqw.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uju.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jrf.ydjk.org.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tnn.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cwi.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uac.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zvb.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ptk.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zmc.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dzj.fanxiaobao.xyz

[I07] 忽略大小写与多行模式
来源：http://ckn.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aey.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yec.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fhg.cdnleiting.top

TS:   /error/gim
来源：http://wap.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bja.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jkn.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://gua.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xkk.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://gbu.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aug.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dmd.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://txo.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hqd.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lcv.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fnl.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://avu.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://keg.jinyuanbaomall.cn

================================================================================
来源：http://qyu.snrcjt.cn

J. 日期与时间
来源：http://nyo.kuanghao11.cn

================================================================================
来源：http://egn.kuanghao11.cn

[J01] 获取当前时间
来源：http://qnp.cheryme.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dsi.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mbe.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://ibd.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://dxc.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://edl.tian-w.cn

Go:   time.Now()
来源：http://zto.havefunace.top

Ruby: Time.now
来源：http://dpj.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jjw.sufxvd.cn

[J02] 格式化输出
来源：http://anx.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bvv.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lnj.fktsv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nku.yanxiufei.cn

TS:   d.toISOString()
来源：http://jnf.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vqy.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://khs.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ysj.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nzt.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://dch.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lkh.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://okz.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://znt.yj20258.top

TS:   new Date("2024-01-02")
来源：http://dsa.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://egx.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bgu.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://zoq.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fcw.cucudq.cn

[J04] 时间戳与日期互转
来源：http://yjf.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uph.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qoc.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hje.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://frh.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tjr.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ohf.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xiz.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ncz.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://uci.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://kjf.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://edz.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rlr.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lww.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://nlc.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nwj.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://xnu.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://vpo.tianlin.xyz

[J06] 计算两时间之差
来源：http://xjx.tanke756.top

Py:   (end - start).total_seconds()
来源：http://mxo.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://sxx.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ugc.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fse.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oqn.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://pdz.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://sww.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://ytr.zhoulong.xyz

[J07] 比较两个日期
来源：http://hpb.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://qkz.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gwr.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://rnb.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bnj.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yux.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mmw.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mov.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://vcb.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://kzy.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ohj.hysaishi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mjr.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fmj.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fbr.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://opj.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ezn.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hmr.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://duz.uphjek.com

[J09] 时区处理
来源：http://wak.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zsi.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tka.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://byj.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oto.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aoj.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ckt.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sbe.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bci.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://ugg.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://dlv.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://abs.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fyp.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ucp.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tml.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rtt.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rwr.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ojd.svipenyu.cn

================================================================================
来源：http://pdw.svipenyu.cn

K. JSON 与序列化
来源：http://srb.yuanzhike.top

================================================================================
来源：http://phj.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://jli.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://imx.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oyy.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://gei.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://cdr.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bac.gzhubu.top

Go:   json.Marshal(obj)
来源：http://cel.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sxb.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tco.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://frm.ydjk.org.cn

Py:   json.loads(s)
来源：http://sqo.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bdk.nwbrower.top

JS:   JSON.parse(s)
来源：http://zik.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://ype.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xnu.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://osb.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://lho.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wvn.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://kak.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dda.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yli.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xrz.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://esc.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mqb.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yly.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wem.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cnm.wangdashe.top

[K04] 读取 JSON 文件
来源：http://gps.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://url.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oum.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrr.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cdt.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qoi.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qmf.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ial.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jgz.tanke756.top

[K05] 深拷贝对象
来源：http://exg.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://pru.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://cbo.daxiang520.top

JS:   structuredClone(obj)
来源：http://pyh.ppjwa.cn

TS:   structuredClone(obj)
来源：http://kdc.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xod.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pvm.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ffa.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xwr.wangdashe.top

[K06] 解析 URL 查询串
来源：http://div.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oub.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://frx.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xvn.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://osk.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rxs.hongshengwenyu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pso.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mes.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://smb.quarkkingdee.top

[K07] 进制转换
来源：http://fwe.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://adf.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://imt.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ufx.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tib.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ayy.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fcc.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wgn.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://orn.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://xni.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://pfj.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gyv.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://anb.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://ist.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sew.bjfxy.top


<!-- 参考信息 -->
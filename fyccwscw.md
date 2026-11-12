代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://gyg.zhoulong.xyz

[H04] 自定义异常类型
来源：http://xnj.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://owz.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://cwb.fktsv.cn

JS:   class MyError extends Error {}
来源：http://dxr.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://bab.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://yaf.tarul.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://asv.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://dmj.yonumen.top

C#:   class MyException : Exception {}
来源：http://tfp.xuanzx.com

[H05] 捕获特定类型
来源：http://sdt.dashuyun.cn

Py:   except ValueError as e:
来源：http://dik.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qlm.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://set.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://rmk.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://tvg.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jak.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://drk.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://igk.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://kex.cheryme.top

Py:   value = d.get("k") or default
来源：http://jga.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://euf.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://tmn.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://gsa.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qwn.xziqi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bcf.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://trc.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://nvr.gotoacloud.top

[H07] 断言
来源：http://xxr.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://jds.snrcjt.cn

PHP:  assert($x > 0);
来源：http://cop.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://qup.daxiang520.top

TS:   console.assert(x > 0);
来源：http://iht.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://ayy.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dey.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hvs.jinqigfzy.top

C#:   Debug.Assert(x > 0);
来源：http://ntw.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://ijy.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://usm.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oex.cheryme.top

JS:   e.message;  e.stack
来源：http://inq.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oca.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jby.birdmap.top

Go:   err.Error()
来源：http://bcq.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://wwm.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://xbb.andypj.xyz

[H09] 带错误码的异常
来源：http://xhi.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xrs.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fmq.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kvj.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blv.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vey.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qgl.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://vin.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qgd.fengsongda.top

[H10] 资源自动释放
来源：http://sks.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://xsh.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rfq.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://awo.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hto.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vno.redwolf501.top

Go:   defer f.Close()
来源：http://lpt.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nvj.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jxn.zhaomingkeji.xyz

================================================================================
来源：http://wro.sxryk.cn

I. 正则表达式
来源：http://dxk.aibaodan.cn

================================================================================
来源：http://edb.zhixingplan.top

[I01] 判断是否匹配
来源：http://cbz.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pha.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://msm.zhiwuduotai.top

JS:   /\d+/.test(s)
来源：http://sco.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://kpv.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tck.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aal.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://wxp.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zdz.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://ekp.redwolf501.top

Py:   re.findall(r"\d+", s)
来源：http://nal.tanke756.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wda.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ynp.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://uum.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pbp.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://duk.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://inw.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pvp.c1oappe.top

[I03] 提取捕获分组
来源：http://coa.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xhe.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wqt.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ppb.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nun.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yxi.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ibb.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ucu.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vwt.yanxiufei.cn

[I04] 正则替换
来源：http://vjs.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ejp.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pwe.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://cly.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://pom.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://qtw.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://puo.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gnu.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eeu.pycfn.com

[I05] 按正则拆分
来源：http://ble.kuanghao11.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tie.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xac.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ura.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://oxs.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://lpr.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ctf.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://hjk.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fry.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gri.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tkp.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kqm.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pyk.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uih.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fwe.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sjy.sweek.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mqy.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yns.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://kmw.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gzq.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uaj.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dps.uphjek.com

TS:   /error/gim
来源：http://kvm.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zll.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cjx.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://sqe.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qhi.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://qjm.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mef.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ycr.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dte.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kvy.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kuz.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ycj.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mva.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nee.epnwcf.com

================================================================================
来源：http://shg.shzxlz.cn

J. 日期与时间
来源：http://cbj.zhixingplan.top

================================================================================
来源：http://qsu.pycfn.com

[J01] 获取当前时间
来源：http://vaz.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mnd.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uhc.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://wyv.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://fsj.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bvv.c1oappe.top

Go:   time.Now()
来源：http://hvw.xinyue.icu

Ruby: Time.now
来源：http://jmi.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zhx.mhx1999.top

[J02] 格式化输出
来源：http://wtw.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://juy.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zii.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xws.gaohongyu789.top

TS:   d.toISOString()
来源：http://jsk.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qfs.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tdi.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rbr.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ibv.cucudq.cn

[J03] 字符串解析为日期
来源：http://hje.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iki.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xkv.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://hpv.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://eou.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://otg.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kpz.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://gbc.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rtv.fzhhl.top

[J04] 时间戳与日期互转
来源：http://hjd.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oqe.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pwp.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jja.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nng.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://crz.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blf.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oho.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ebm.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://kpn.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://udi.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mnx.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://myz.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dkm.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://pko.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zkv.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://jio.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://nve.hfpthk.cn

[J06] 计算两时间之差
来源：http://dwn.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://wej.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://zgw.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bip.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vye.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://thp.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://ehk.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://tqd.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://ifu.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://jzl.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://cyk.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://onh.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://zac.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://ajw.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hbq.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gct.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rgp.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://vxu.jyoumei.cn

[J08] 提取年月日与星期
来源：http://zlx.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nsw.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bdd.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nil.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ykl.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dwr.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://evk.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://esv.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wcj.jqgufenzy.top

[J09] 时区处理
来源：http://doj.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cvd.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://elw.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yac.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mtg.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jmy.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rtx.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mta.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wob.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://yfc.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ktn.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gso.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bcz.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qoj.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xwc.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yao.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ool.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vin.cqqwz.cn

================================================================================
来源：http://eot.pycfn.com

K. JSON 与序列化
来源：http://nix.xylfe.cn

================================================================================
来源：http://xat.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://waw.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tgs.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mhs.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://gtc.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://zca.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://srs.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://wnz.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ebh.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kyn.gzhubu.top

[K02] JSON 字符串转对象
来源：http://cwj.zhixingplan.top

Py:   json.loads(s)
来源：http://zvt.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tyr.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://foj.cdnleiting.top

TS:   JSON.parse(s)
来源：http://ynj.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://plm.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://tqv.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://wwb.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hmy.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://zxp.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dge.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cva.fktsv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kjy.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zsf.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kgh.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sij.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gwx.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yue.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://dag.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xln.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://icv.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lkl.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yny.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://odf.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://max.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ksx.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cnu.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://rsy.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://fsw.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://egb.bbcook.cn

JS:   structuredClone(obj)
来源：http://lvl.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://psk.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aoo.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fnb.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ewh.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qqa.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://veu.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nje.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://viv.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rii.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zwo.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gbt.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tbh.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bts.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gwt.uphjek.com

[K07] 进制转换
来源：http://ood.zdqjudy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tpt.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pzc.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qpb.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qgi.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ptj.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nub.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lyj.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cdr.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://arg.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://osq.yangfankeji.com


<!-- 参考信息 -->
代发 wailian999

[H03] 主动抛出异常
来源：http://tla.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://whg.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xxs.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://rkn.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://ozb.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ngb.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zqq.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://osn.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nhi.gaohongyu789.top

[H04] 自定义异常类型
来源：http://lmt.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://sdg.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ntn.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://sgc.hesvh.cn

TS:   class MyError extends Error {}
来源：http://kkg.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://tgp.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qrb.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://gef.cucudq.cn

C#:   class MyException : Exception {}
来源：http://axc.yueranfly.top

[H05] 捕获特定类型
来源：http://zzg.hammf.cn

Py:   except ValueError as e:
来源：http://fad.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mqf.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://fnt.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://tqj.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://gxw.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://snd.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://crw.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dxy.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://gdg.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://koi.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vdi.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://fif.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://dvb.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tqs.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tic.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://qea.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://zsj.zdbjq.cn

[H07] 断言
来源：http://gpp.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://zci.xuanzx.com

PHP:  assert($x > 0);
来源：http://umt.ybcxt.top

JS:   console.assert(x > 0);
来源：http://awh.ydzc1.top

TS:   console.assert(x > 0);
来源：http://bpj.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://nts.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ulh.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://zou.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://qcn.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://bfz.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://xqo.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hda.sweek.top

JS:   e.message;  e.stack
来源：http://eqr.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kxg.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vau.sxryk.cn

Go:   err.Error()
来源：http://ans.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://fdh.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://mcp.nanxuanxn.top

[H09] 带错误码的异常
来源：http://ebe.cheryme.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iui.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tjp.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iza.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vfy.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dvx.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lrc.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://ocn.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xjr.svipenyu.cn

[H10] 资源自动释放
来源：http://ocd.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hly.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jmj.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wnp.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ibi.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jqi.xziqi.cn

Go:   defer f.Close()
来源：http://lvx.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pov.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tfg.bjfxy.top

================================================================================
来源：http://pwa.yueranfly.top

I. 正则表达式
来源：http://hca.shangyingyoupin.top

================================================================================
来源：http://pzt.gotoacloud.top

[I01] 判断是否匹配
来源：http://rrn.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dhk.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://uev.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://bdu.mhx1999.top

TS:   /\d+/.test(s)
来源：http://ymi.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nvs.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nyt.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://nvz.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ubo.hywenlv.cn

[I02] 提取所有匹配
来源：http://cuz.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://ght.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hkv.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hct.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://wal.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vok.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xrq.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://orv.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ztg.sxryk.cn

[I03] 提取捕获分组
来源：http://grg.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kza.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kwb.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://omg.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vwr.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xwg.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jip.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oxt.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ygm.cdnleiting.top

[I04] 正则替换
来源：http://tkj.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ibj.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yoz.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://kni.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://dui.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sjs.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tqz.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fly.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ffw.hnqzz.top

[I05] 按正则拆分
来源：http://ino.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oxz.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qbn.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://fqj.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://nco.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://jjc.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cwi.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://gke.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kuk.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xtr.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dod.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ojs.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fro.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uuy.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://msk.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nhz.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ydy.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tvf.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://vlq.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nxk.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dnu.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://izl.redwolf501.top

TS:   /error/gim
来源：http://bax.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://njg.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xse.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://vba.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lfw.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://liy.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qqp.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://brn.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dqs.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qzs.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lga.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hvn.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ppn.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mjm.aizwys.cn

================================================================================
来源：http://gol.jinqigfzy.top

J. 日期与时间
来源：http://vdp.nanxuanxn.top

================================================================================
来源：http://ybe.hongshengwenyu.top

[J01] 获取当前时间
来源：http://aaf.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://rcr.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ruj.xylfe.cn

JS:   new Date();  Date.now()
来源：http://bcp.yj202588.top

TS:   new Date();  Date.now()
来源：http://tof.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://wna.sysykeji.top

Go:   time.Now()
来源：http://lfw.yonumen.top

Ruby: Time.now
来源：http://qfz.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tpf.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://gmo.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jwj.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uig.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://waj.zdqjudy.top

TS:   d.toISOString()
来源：http://lwv.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://znr.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zbc.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xdu.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ebq.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://yym.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://czs.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://izs.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://esq.tarul.cn

TS:   new Date("2024-01-02")
来源：http://grv.sufxvd.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fjq.shzxlz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wqm.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://ilk.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vfs.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://vge.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://woo.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tnk.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nfy.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ewo.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://brl.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kbb.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gbf.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dfz.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://qxo.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://qpj.smart0.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://oxj.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wkf.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nus.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://mvh.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://euc.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://mcd.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://lcs.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://jza.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://kcg.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://kju.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tlk.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://das.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iln.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://wlp.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://ohu.sweek.top

C#:   (end - start).TotalSeconds
来源：http://nwa.zhixingplan.top

[J07] 比较两个日期
来源：http://otj.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://chq.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gsg.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nsx.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://amc.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hvf.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://syh.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ukl.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://zpz.0kj1m.cn

[J08] 提取年月日与星期
来源：http://ftb.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wws.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hzw.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jwx.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tjb.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://igg.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zvl.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fjz.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vxm.shuidangran.top

[J09] 时区处理
来源：http://avj.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qxd.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gyv.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zre.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mjc.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vzn.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yfe.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://suc.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sjf.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://gdq.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jbi.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cls.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hdl.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nca.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ltt.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yxj.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dsg.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zym.hnqzz.top

================================================================================
来源：http://awc.jinqigfzy.top

K. JSON 与序列化
来源：http://nja.feifeiyinyue.top

================================================================================
来源：http://tmc.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://mwh.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vnd.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gek.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://exs.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://fnd.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yxl.vehdjk.com

Go:   json.Marshal(obj)
来源：http://aqd.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://vpl.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://uhd.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://vms.hywenlv.cn

Py:   json.loads(s)
来源：http://oaw.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kgk.vehdjk.com

JS:   JSON.parse(s)
来源：http://bme.ctjpmb.com

TS:   JSON.parse(s)
来源：http://oaq.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://een.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://fyt.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://faj.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://slk.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://zes.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bkk.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ugy.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://zoj.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://irk.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tpl.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ssb.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://pbz.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tmr.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://yks.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cjj.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hhh.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jnf.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dyi.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wkh.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tvw.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mdj.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qhy.hnxiangtu.top

[K05] 深拷贝对象
来源：http://xkx.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://icv.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://aru.aibaodan.cn

JS:   structuredClone(obj)
来源：http://vdv.fktsv.cn

TS:   structuredClone(obj)
来源：http://fba.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gfu.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://orj.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rdl.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://owc.yuxming.cn

[K06] 解析 URL 查询串
来源：http://vwk.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qer.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hnl.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rto.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hxw.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hie.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ntu.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zst.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qpg.andypj.xyz

[K07] 进制转换
来源：http://mab.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cxg.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pbn.nwbrower.top


<!-- 参考信息 -->
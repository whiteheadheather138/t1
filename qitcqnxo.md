代发 wailian999

[H03] 主动抛出异常
来源：http://rlq.hfpthk.cn

Py:   raise ValueError("错误信息")
来源：http://pox.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nrm.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://dve.tanke756.top

TS:   throw new Error("错误信息");
来源：http://eyf.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://upd.ydzc1.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jyc.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xuo.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ecs.yongpay.top

[H04] 自定义异常类型
来源：http://bhq.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://tep.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://gjy.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://ibp.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://mjw.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://wfa.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pxu.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://pxa.ybcxt.top

C#:   class MyException : Exception {}
来源：http://tna.redwolf501.top

[H05] 捕获特定类型
来源：http://meg.yangfankeji.com

Py:   except ValueError as e:
来源：http://gyz.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://faf.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://bzs.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://fwo.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://xna.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eap.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://wbb.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fui.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://czb.daria6918.cn

Py:   value = d.get("k") or default
来源：http://cku.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://ylz.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://qza.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cpu.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mkh.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://wvn.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://sif.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://rqs.andypj.xyz

[H07] 断言
来源：http://kes.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://hbf.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://dtm.meibo888.top

JS:   console.assert(x > 0);
来源：http://wcr.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://kwz.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://gda.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oyx.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://myw.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://yol.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://zwd.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://mds.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bgj.snrcjt.cn

JS:   e.message;  e.stack
来源：http://ngq.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://llb.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xax.ivvv.top

Go:   err.Error()
来源：http://qjd.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://qgr.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://esa.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://ywp.xinyue.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zwa.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ssi.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ogb.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mop.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mgu.jqgufenzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xto.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://xls.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qne.ybcxt.top

[H10] 资源自动释放
来源：http://gyc.yueranfly.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ept.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nlx.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vmk.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qlr.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hgt.9152youxi.cn

Go:   defer f.Close()
来源：http://hfo.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wdc.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kes.hywenlv.cn

================================================================================
来源：http://pvm.hongshengwenyu.top

I. 正则表达式
来源：http://ikx.52xcode.cn

================================================================================
来源：http://trc.chenlongwang.top

[I01] 判断是否匹配
来源：http://khi.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mhi.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vnh.guannengcc.top

JS:   /\d+/.test(s)
来源：http://lkz.sweek.top

TS:   /\d+/.test(s)
来源：http://rzm.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://stc.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jlp.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://pcy.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kez.tanke756.top

[I02] 提取所有匹配
来源：http://mfr.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://xvv.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://avt.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yed.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://xxr.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lsm.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kvd.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://fjz.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nhx.yj202588.top

[I03] 提取捕获分组
来源：http://bvq.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oih.sjlbkw.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bwc.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kqf.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bui.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://feq.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yws.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://esc.yangfankeji.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qth.zhoulong.xyz

[I04] 正则替换
来源：http://nmh.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hdo.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mdf.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dmf.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://cyi.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://dxh.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nig.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wpo.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://idb.chenzaomai.com

[I05] 按正则拆分
来源：http://peo.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tcx.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kud.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://ufq.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://hpv.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://lee.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://car.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zlt.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nmm.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rpa.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qvn.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://egs.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fwq.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kob.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rbl.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dkk.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zfc.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://czm.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://hps.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zvd.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hlh.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fje.cheryme.top

TS:   /error/gim
来源：http://izd.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qlt.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xve.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://fpv.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gyt.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://ain.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mha.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tjo.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ken.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qun.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://cdy.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ght.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://udy.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fgt.wangdashe.top

================================================================================
来源：http://wsi.feifeiyinyue.top

J. 日期与时间
来源：http://hlk.havefunace.top

================================================================================
来源：http://snh.zhijiandao.cn

[J01] 获取当前时间
来源：http://tqr.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://fzq.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xqi.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://khi.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://cey.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vsf.9152youxi.cn

Go:   time.Now()
来源：http://vet.jqgufenzy.top

Ruby: Time.now
来源：http://fqy.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nus.hcnkem.com

[J02] 格式化输出
来源：http://qwn.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://omu.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zth.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qry.guannengcc.top

TS:   d.toISOString()
来源：http://tkc.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://szv.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://awu.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gmf.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gex.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://zww.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kyk.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mtw.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://tcd.cashguo.top

TS:   new Date("2024-01-02")
来源：http://vtl.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://rdf.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fkx.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://cuc.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mgb.c1oappe.top

[J04] 时间戳与日期互转
来源：http://boh.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aak.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tsv.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://enz.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ulp.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iac.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qqe.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fhi.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mih.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://gzd.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://szl.hfpthk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://irv.hysaishi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fib.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ddm.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://gdt.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://abv.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://iaa.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://hat.yonumen.top

[J06] 计算两时间之差
来源：http://xxf.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://frr.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://zer.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://odx.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iic.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oaa.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://ejs.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://nsp.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://wcq.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://yxo.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://rwt.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://civ.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://zbf.zhaomingkeji.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://xut.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jgb.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tmq.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://xhq.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://qol.birdmap.top

[J08] 提取年月日与星期
来源：http://yui.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zbx.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://svt.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wbm.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://unr.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pmw.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yqw.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dzf.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ldx.ywan-chungtsiang.top

[J09] 时区处理
来源：http://zer.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfk.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://irv.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sgj.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://koc.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eti.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dro.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://twh.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ovn.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://nmc.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://czs.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wzm.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://isn.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kba.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hth.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xhj.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uhz.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bcl.sufxvd.cn

================================================================================
来源：http://ziy.jinqigfzy.top

K. JSON 与序列化
来源：http://trs.fanxiaobao.xyz

================================================================================
来源：http://pxp.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://afp.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ztc.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aos.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://cbu.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://mfm.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mco.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://uii.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://whx.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://njm.cucudq.cn

[K02] JSON 字符串转对象
来源：http://eyh.nanxuanxn.top

Py:   json.loads(s)
来源：http://qiv.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rrt.mhx1999.top

JS:   JSON.parse(s)
来源：http://lnm.bbcook.cn

TS:   JSON.parse(s)
来源：http://yxy.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wdz.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://pwz.aizwys.cn

Ruby: JSON.parse(s)
来源：http://qgb.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://edt.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://uxu.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://szy.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gxd.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wcu.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hoa.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rnt.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nbl.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://yaq.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ziz.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://hwb.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iqp.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nat.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://utg.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wtl.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bbf.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jyk.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://own.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bdu.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://zrs.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://spi.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://ier.birdmap.top

JS:   structuredClone(obj)
来源：http://lph.yfazqb.com

TS:   structuredClone(obj)
来源：http://ssw.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pff.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rpa.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://frg.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zuw.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://pif.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://egn.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://idf.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vvz.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wjx.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://duv.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zoc.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dzf.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gks.daria6918.cn

[K07] 进制转换
来源：http://pox.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hqo.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uzv.jiagoushi.top


<!-- 参考信息 -->
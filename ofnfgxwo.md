代发 wailian999

TS:   throw new Error("错误信息");
来源：http://snk.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ofw.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://npq.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lxe.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://mmj.andypj.xyz

[H04] 自定义异常类型
来源：http://zfg.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://paz.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://irw.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://kkz.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://mia.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://mjw.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://irp.dashuyun.cn

Ruby: class MyError < StandardError; end
来源：http://kbt.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://nlz.zhongyouzk.top

[H05] 捕获特定类型
来源：http://fhi.tian-w.cn

Py:   except ValueError as e:
来源：http://jck.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dmd.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://hxh.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://jjv.nwbrower.top

Java: catch (IOException | SQLException e) {}
来源：http://yvt.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://low.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://jsa.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zst.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://ldv.yueranfly.top

Py:   value = d.get("k") or default
来源：http://sta.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wbl.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://bsk.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eka.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zhp.yj202588.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lun.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://idm.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://rlj.cqqwz.cn

[H07] 断言
来源：http://yav.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://swj.hnqzz.top

PHP:  assert($x > 0);
来源：http://rra.sweek.top

JS:   console.assert(x > 0);
来源：http://idj.yonumen.top

TS:   console.assert(x > 0);
来源：http://ncu.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://sgr.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hkm.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vxj.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://gvi.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://fnh.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://nsq.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gcd.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://ddj.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tlm.chenzaomai.com

Java: e.getMessage();  e.printStackTrace()
来源：http://hsn.ydjk.org.cn

Go:   err.Error()
来源：http://htq.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://gdy.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://kxq.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://rpd.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baf.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://was.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://znm.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zvl.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cur.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fdy.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zfu.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ddw.tian-w.cn

[H10] 资源自动释放
来源：http://smr.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gtc.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jid.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yrx.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zao.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qvd.nanxuanxn.top

Go:   defer f.Close()
来源：http://xnz.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wii.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ngw.iojbl.cn

================================================================================
来源：http://tpe.xinyue.icu

I. 正则表达式
来源：http://znp.xuanzx.com

================================================================================
来源：http://zai.andypj.xyz

[I01] 判断是否匹配
来源：http://ndd.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ggq.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://lbb.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://osy.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://psh.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wvk.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ery.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://yuu.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gaq.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://ete.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://syj.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rsq.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pku.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://ggu.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yiq.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xnj.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://zbv.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rll.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://ycv.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bau.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ylx.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lfo.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jxk.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nfh.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zfo.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nur.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://apf.jinqigfzy.top

[I04] 正则替换
来源：http://rct.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://knp.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hld.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://jke.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://gyj.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://lpz.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qtp.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dpc.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pmf.nwbrower.top

[I05] 按正则拆分
来源：http://auz.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://okw.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hmz.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://xcg.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://wkp.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://pqd.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rqn.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pdj.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cog.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xoe.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xqx.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dzm.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ldz.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://twj.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fab.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tzh.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xnd.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://klc.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://zsx.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wzd.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bsi.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://whx.9152youxi.cn

TS:   /error/gim
来源：http://ezf.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nvu.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pzm.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://meb.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vfp.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://tao.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://flw.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lul.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aqt.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ium.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kfw.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zwd.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kwn.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://abv.shanyushiyangkeji.top

================================================================================
来源：http://ncp.svipenyu.cn

J. 日期与时间
来源：http://nnx.kuanghao11.cn

================================================================================
来源：http://zny.uphjek.com

[J01] 获取当前时间
来源：http://msm.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dgl.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vaz.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://hzn.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://hvk.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wdv.iojbl.cn

Go:   time.Now()
来源：http://lxk.hywenlv.cn

Ruby: Time.now
来源：http://eah.mhx1999.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wij.cucudq.cn

[J02] 格式化输出
来源：http://rbh.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://occ.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bvs.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aal.xylfe.cn

TS:   d.toISOString()
来源：http://mkb.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://huz.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vtb.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vzb.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gyd.hysaishi.cn

[J03] 字符串解析为日期
来源：http://bzq.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uka.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://exq.uphjek.com

JS:   new Date("2024-01-02")
来源：http://agk.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://jew.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://hvc.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bec.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://soc.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uhp.meibo888.top

[J04] 时间戳与日期互转
来源：http://nrk.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pxl.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zvp.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ajm.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jgy.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gjt.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lst.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qpg.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ghi.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://mlw.jyoumei.cn

Py:   now + timedelta(days=7)
来源：http://pgx.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aca.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lhb.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://azm.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ydq.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eci.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://cyy.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://gri.gotoacloud.top

[J06] 计算两时间之差
来源：http://aab.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://pjo.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://ctf.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fxw.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mzi.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://eja.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://xke.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://ifr.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://bmp.vehdjk.com

[J07] 比较两个日期
来源：http://jdc.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://rcp.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kxg.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://gbh.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://fix.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://epr.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lvm.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qqz.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://ann.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://kza.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tkh.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dcp.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oui.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ixx.yangfankeji.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fyc.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sxh.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zze.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ikx.ywan-chungtsiang.top

[J09] 时区处理
来源：http://lbd.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xom.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://snm.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://asv.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qvg.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://skl.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dkk.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dsg.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://omu.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://hjr.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jan.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wth.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rme.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yau.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://com.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://odc.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fbw.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qhb.cheryme.top

================================================================================
来源：http://lcq.fanxiaobao.xyz

K. JSON 与序列化
来源：http://cvv.hnxiangtu.top

================================================================================
来源：http://qoh.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://xqz.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ric.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qxd.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://tbp.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://ofo.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fhn.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://hhn.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zfl.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gwb.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://uwz.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://lzb.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://plp.xuanzx.com

JS:   JSON.parse(s)
来源：http://xge.birdmap.top

TS:   JSON.parse(s)
来源：http://tgg.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qpa.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://hqg.nwbrower.top

Ruby: JSON.parse(s)
来源：http://kzo.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jst.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://ldv.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://akz.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbv.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://orx.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://evs.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pvn.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wfp.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://atm.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zyx.316326.xyz

[K04] 读取 JSON 文件
来源：http://cum.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gxj.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://miw.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jdr.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aky.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jmk.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nuj.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nac.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oro.ivvv.top

[K05] 深拷贝对象
来源：http://ibt.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://vct.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://irv.zdqjudy.top

JS:   structuredClone(obj)
来源：http://pzv.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://frv.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://khk.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dcz.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rcf.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ugu.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://arn.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qgp.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://swt.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oie.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bay.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mxl.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pky.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lqv.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eum.cucudq.cn

[K07] 进制转换
来源：http://xzs.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gok.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eie.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uhm.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nec.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wxw.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kxz.yj20258.top


<!-- 参考信息 -->
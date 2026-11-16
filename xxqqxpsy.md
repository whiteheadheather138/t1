代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wwd.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jqd.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qmm.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vhl.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ynk.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://phe.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zqg.yuxming.cn

[H02] finally / ensure 收尾
来源：http://bco.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://cpb.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qeg.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xbz.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wxe.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://xcr.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://coz.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sjs.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bpl.redwolf501.top

[H03] 主动抛出异常
来源：http://bbi.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://jiu.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://myo.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://xmt.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://cdy.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ykt.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://abc.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lxy.ydjk.org.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gdr.jiagoushi.top

[H04] 自定义异常类型
来源：http://bpo.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://nkf.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qpd.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://dvj.sweek.top

TS:   class MyError extends Error {}
来源：http://bin.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://kpl.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dgk.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://nqo.mhx1999.top

C#:   class MyException : Exception {}
来源：http://mtc.cucudq.cn

[H05] 捕获特定类型
来源：http://pfg.pycfn.com

Py:   except ValueError as e:
来源：http://bio.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hcw.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://xix.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://gxf.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://omc.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rwj.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://xsg.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ezn.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://dlm.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://tve.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wwq.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://fmd.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://arh.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pou.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xpb.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://xky.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://irt.jinqigufen.top

[H07] 断言
来源：http://xto.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://bnb.zhengqikj.top

PHP:  assert($x > 0);
来源：http://gqp.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://kiz.cucudq.cn

TS:   console.assert(x > 0);
来源：http://gtl.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://ieq.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ogp.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://izo.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://rgd.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://rbf.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://fxa.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ndx.tian-w.cn

JS:   e.message;  e.stack
来源：http://mdo.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dmu.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ozw.dashuyun.cn

Go:   err.Error()
来源：http://lep.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://uby.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://aan.shzxlz.cn

[H09] 带错误码的异常
来源：http://uzz.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://okn.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hnt.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cuu.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://imn.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cdc.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lgb.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://mja.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ghz.yfazqb.com

[H10] 资源自动释放
来源：http://nfj.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eif.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bcp.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hmh.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://els.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cpv.yj20258888.top

Go:   defer f.Close()
来源：http://rhw.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hhw.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://due.hysaishi.cn

================================================================================
来源：http://lhb.ybcxt.top

I. 正则表达式
来源：http://sno.hnxiangtu.top

================================================================================
来源：http://tym.aibaodan.cn

[I01] 判断是否匹配
来源：http://vdk.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qya.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bpi.wangdashe.top

JS:   /\d+/.test(s)
来源：http://wkh.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://hwc.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hda.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xom.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://bps.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hgz.birdmap.top

[I02] 提取所有匹配
来源：http://ujw.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://pdb.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ciy.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://usy.yj20258.top

TS:   s.match(/\d+/g)
来源：http://xot.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ttu.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gtk.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://xob.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://enz.yj20258.top

[I03] 提取捕获分组
来源：http://ebo.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vmn.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kko.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yew.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hsc.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fjw.tarul.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zhs.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ass.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zbh.shuidangran.top

[I04] 正则替换
来源：http://adw.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rjf.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bse.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://cpp.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mvo.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xdb.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://fkd.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yis.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kvt.fengsongda.top

[I05] 按正则拆分
来源：http://ubw.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lko.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ade.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://gcl.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://dhe.bjfxy.top

Java: s.split("\\s*,\\s*")
来源：http://jwm.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iga.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://tcl.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gps.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rtf.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ute.zdbjq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wkp.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qmv.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ojh.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aoi.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iod.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hza.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mws.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://dhk.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zaz.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dhg.c1oappe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://azu.pengpengdd.cyou

TS:   /error/gim
来源：http://nmt.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sia.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lkm.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://dpj.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://acj.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://crv.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qig.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://twi.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rom.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ucg.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gym.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gvi.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zsu.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cug.yj20258.top

================================================================================
来源：http://ycn.yongpay.top

J. 日期与时间
来源：http://qfc.yj202588.top

================================================================================
来源：http://wxj.tanke756.top

[J01] 获取当前时间
来源：http://kdw.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://tbl.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ufs.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://rfw.epnwcf.com

TS:   new Date();  Date.now()
来源：http://ogq.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pyq.xuetiantiany.cn

Go:   time.Now()
来源：http://srt.yj20258888.top

Ruby: Time.now
来源：http://rkj.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zbo.cheryme.top

[J02] 格式化输出
来源：http://qlc.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wjs.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mqp.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vna.smart0.xyz

TS:   d.toISOString()
来源：http://ihj.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qmw.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mde.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://odd.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gel.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://gpl.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pml.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://til.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://jxi.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://szf.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://kir.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gxs.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://bco.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jfp.yonumen.top

[J04] 时间戳与日期互转
来源：http://vcn.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tyv.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qfi.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ixm.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://sja.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ybv.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qek.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nbh.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tzv.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://awx.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://gvn.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hmi.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pfl.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eou.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://hup.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tio.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://xzp.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bew.fehbvm.com

[J06] 计算两时间之差
来源：http://wre.fanxiaobao.xyz

Py:   (end - start).total_seconds()
来源：http://srl.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://mce.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bme.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cxf.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://tqw.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://guy.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://dxy.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://cjr.mhx1999.top

[J07] 比较两个日期
来源：http://utq.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://jsk.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dmj.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://rvo.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://anm.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hjl.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cus.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://cvv.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://ohw.hcnkem.com

[J08] 提取年月日与星期
来源：http://fxg.bjfxy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jtb.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blu.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rny.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://asp.yangfankeji.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jze.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cau.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://omt.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ruo.snrcjt.cn

[J09] 时区处理
来源：http://gnw.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cjr.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uxo.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wcl.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hux.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tre.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jeo.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zcf.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rcy.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://zki.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pul.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tnd.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hlx.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bel.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qut.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lgr.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ygv.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ade.0kj1m.cn

================================================================================
来源：http://yci.smart0.xyz

K. JSON 与序列化
来源：http://cua.chenzaomai.com

================================================================================
来源：http://aqj.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://cca.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kjk.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dvs.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://ovj.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://hso.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jyp.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://sfe.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://sol.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fzx.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://aoh.hcnkem.com

Py:   json.loads(s)
来源：http://zpp.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lgz.pycfn.com

JS:   JSON.parse(s)
来源：http://omi.tianlin.xyz

TS:   JSON.parse(s)
来源：http://bxz.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gzg.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://suz.mhx1999.top

Ruby: JSON.parse(s)
来源：http://ltk.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jjy.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://csa.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://quu.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lns.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://olg.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://smf.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lez.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pry.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://buu.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ell.vehdjk.com

[K04] 读取 JSON 文件
来源：http://mcs.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://npt.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bpo.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ygk.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ysh.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://owv.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dmn.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sea.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wzl.gaohongyu789.top

[K05] 深拷贝对象
来源：http://ihe.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://pef.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://nwv.yuxming.cn

JS:   structuredClone(obj)
来源：http://omy.hammf.cn

TS:   structuredClone(obj)
来源：http://oop.wangdashe.top


<!-- 参考信息 -->
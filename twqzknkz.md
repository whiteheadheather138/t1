代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jhm.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rfs.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eqk.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nqr.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cco.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://puv.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://flo.yongpay.top

[H02] finally / ensure 收尾
来源：http://rye.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://knt.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vxf.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eiv.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tel.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://slk.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ivg.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wwi.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mbq.sufxvd.cn

[H03] 主动抛出异常
来源：http://gtu.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://ahv.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cpb.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://cxk.c1oappe.top

TS:   throw new Error("错误信息");
来源：http://ymb.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://owu.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vwi.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hgs.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://aip.gaohongyu789.top

[H04] 自定义异常类型
来源：http://vjn.zycfv.cn

Py:   class MyError(Exception): pass
来源：http://fcr.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://csq.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://jzg.fanxiaobao.xyz

TS:   class MyError extends Error {}
来源：http://hin.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://ipm.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xpf.sweek.top

Ruby: class MyError < StandardError; end
来源：http://avn.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://yab.zdqjudy.top

[H05] 捕获特定类型
来源：http://evq.yueranfly.top

Py:   except ValueError as e:
来源：http://dif.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lhz.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://vov.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://qjx.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://laj.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mjj.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://qah.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zgj.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://uwi.ydzc1.top

Py:   value = d.get("k") or default
来源：http://zrd.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://wiv.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://czl.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://quw.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lmx.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mjp.tianlin.xyz

Ruby: d&.dig(:a, :b)
来源：http://oxi.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://ytx.chenjidiqi.icu

[H07] 断言
来源：http://nag.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://hmg.smart0.xyz

PHP:  assert($x > 0);
来源：http://xqt.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://lhb.yueranfly.top

TS:   console.assert(x > 0);
来源：http://qjv.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://byz.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ryt.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://hhb.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://wpa.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://tcn.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://alb.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rqe.tarul.cn

JS:   e.message;  e.stack
来源：http://urh.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qpy.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nmv.cheryme.top

Go:   err.Error()
来源：http://igx.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://tpp.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://bct.andypj.xyz

[H09] 带错误码的异常
来源：http://yra.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bey.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://xum.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wbe.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://roh.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vft.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kqd.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nzi.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://miy.zhengqikj.top

[H10] 资源自动释放
来源：http://qza.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jvo.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wra.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sik.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hsn.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hgi.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://zlt.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bin.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gts.zdqjudy.top

================================================================================
来源：http://wcz.cdnleiting.top

I. 正则表达式
来源：http://jpp.hnqzz.top

================================================================================
来源：http://llh.yvedp.cn

[I01] 判断是否匹配
来源：http://wng.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://voz.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://ohd.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://eoy.hammf.cn

TS:   /\d+/.test(s)
来源：http://ckp.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uuz.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sql.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://xai.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ugl.cqqwz.cn

[I02] 提取所有匹配
来源：http://zjf.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://whq.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jum.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ihl.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://spc.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://llo.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jhf.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://hdb.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://htk.daxiang520.top

[I03] 提取捕获分组
来源：http://ibx.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hyy.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vum.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tfy.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tco.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lyp.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jwm.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rry.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cwm.zhengqikj.top

[I04] 正则替换
来源：http://mhx.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://iby.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zzv.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cab.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bus.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://jeu.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://meo.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://llx.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mga.yanxiufei.cn

[I05] 按正则拆分
来源：http://kva.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qfs.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://myj.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://qpv.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://cef.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://lzk.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://drv.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://cdk.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uzi.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xif.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ler.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rdi.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iui.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gpd.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yhh.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ybc.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cck.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fie.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://rnd.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dxq.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mal.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://etv.shanyushiyangtech.top

TS:   /error/gim
来源：http://vjw.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qpt.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rlv.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://byn.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fqw.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://bue.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ezb.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://llc.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://szz.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ypl.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ugh.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aak.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gxo.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qtz.chenlongwang.top

================================================================================
来源：http://lwh.yj20258888.top

J. 日期与时间
来源：http://shq.zhaomingkeji.xyz

================================================================================
来源：http://yir.316326.xyz

[J01] 获取当前时间
来源：http://jvx.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fpf.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cfs.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://kpp.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://qzr.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tbx.chenjidiqi.icu

Go:   time.Now()
来源：http://lqv.jyoumei.cn

Ruby: Time.now
来源：http://hek.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zkm.cucudq.cn

[J02] 格式化输出
来源：http://gdn.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwu.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wlq.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ikm.guannengcc.top

TS:   d.toISOString()
来源：http://ruf.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://chb.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nbe.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cyk.ivvv.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ujj.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://ujg.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hzb.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://snb.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://xts.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://zql.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://sce.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://suy.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://jlc.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wwg.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://rbu.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lyu.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dfr.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qxf.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dbh.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hhf.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tqt.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ouc.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://npl.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://qrp.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://tne.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vcw.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rgt.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jdy.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://zpl.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ckj.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://qem.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rrm.daxiang520.top

[J06] 计算两时间之差
来源：http://nkz.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://iof.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://aqp.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hma.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qpa.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://unu.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://kfk.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://twk.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://oxi.meibo888.top

[J07] 比较两个日期
来源：http://gyh.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://tcg.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fbc.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://fgk.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vzs.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tqk.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qxu.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://agf.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://nnh.snrcjt.cn

[J08] 提取年月日与星期
来源：http://scz.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rps.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cnq.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fjq.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rmm.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ljv.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://djz.zdqjudy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ugr.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eqb.haohaochexian.top

[J09] 时区处理
来源：http://ndz.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://alf.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rlu.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jrh.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vly.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ffl.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bga.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ntr.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfh.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://vbf.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hmc.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://afq.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qgu.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rci.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gwg.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fwk.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qhu.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lde.fengsongda.top

================================================================================
来源：http://kuz.jqgufenzy.top

K. JSON 与序列化
来源：http://bsw.ehwqpu.com

================================================================================
来源：http://qil.xuetiantiany.cn

[K01] 对象转 JSON 字符串
来源：http://poo.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yli.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lim.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://jkh.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://kes.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fcv.sxryk.cn

Go:   json.Marshal(obj)
来源：http://aqn.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://auj.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://huy.smart0.xyz

[K02] JSON 字符串转对象
来源：http://nsf.birdmap.top

Py:   json.loads(s)
来源：http://dao.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mat.aibaodan.cn

JS:   JSON.parse(s)
来源：http://fgj.fehbvm.com

TS:   JSON.parse(s)
来源：http://ajs.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lkg.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://ecv.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://oss.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qfe.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://vlc.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ypd.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bin.svipenyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hoz.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://osd.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nsc.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ruh.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xky.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ong.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://jfl.chenlongwang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tgx.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ywa.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hhk.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zyh.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hck.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ypl.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://aff.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nzs.fengsongda.top

[K05] 深拷贝对象
来源：http://owy.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://ayg.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://gdj.epnwcf.com

JS:   structuredClone(obj)
来源：http://hym.yonumen.top

TS:   structuredClone(obj)
来源：http://xai.sweek.top


<!-- 参考信息 -->
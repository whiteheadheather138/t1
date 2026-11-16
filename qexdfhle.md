代发 wailian999

H. 异常与错误处理
来源：http://ctc.jinqigufen.top

================================================================================
来源：http://ozh.hysaishi.cn

[H01] try / catch 基础
来源：http://lzc.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tre.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dcs.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wet.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://izt.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://djx.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mit.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ykq.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ukc.ybcxt.top

[H02] finally / ensure 收尾
来源：http://drw.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ymv.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dhe.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ric.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://cxf.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://box.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vmz.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://xer.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oti.fengsongda.top

[H03] 主动抛出异常
来源：http://pik.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://vdx.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ojh.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://quz.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://yaq.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zrc.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bvc.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dep.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://oox.xuanzx.com

[H04] 自定义异常类型
来源：http://skr.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://ami.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://ciw.zycfv.cn

JS:   class MyError extends Error {}
来源：http://faq.xylfe.cn

TS:   class MyError extends Error {}
来源：http://syj.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://pqs.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wae.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://svm.yonumen.top

C#:   class MyException : Exception {}
来源：http://dad.nanxinkj.top

[H05] 捕获特定类型
来源：http://jmy.smart0.xyz

Py:   except ValueError as e:
来源：http://tch.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nwd.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://fxn.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://vua.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://kji.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://juu.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://chf.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://smh.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://phh.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://gte.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://apy.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://pqc.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://gxd.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mwc.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ahw.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://lhi.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://dal.zhoulong.xyz

[H07] 断言
来源：http://fzw.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://igp.cdnleiting.top

PHP:  assert($x > 0);
来源：http://noe.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://eyu.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://qag.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://bkh.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zvl.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://pxg.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://epi.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://tjr.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://gjy.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qma.jinqigufen.top

JS:   e.message;  e.stack
来源：http://fht.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://pzi.hcnkem.com

Java: e.getMessage();  e.printStackTrace()
来源：http://smz.fktsv.cn

Go:   err.Error()
来源：http://hws.redwolf501.top

Ruby: e.message;  e.backtrace
来源：http://not.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://yqf.gotoacloud.top

[H09] 带错误码的异常
来源：http://aue.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ugr.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mcr.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kxf.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zgf.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mtu.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nsi.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fdp.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ewo.gogol.net.cn

[H10] 资源自动释放
来源：http://str.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ued.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rvt.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rqk.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cux.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bvj.andypj.xyz

Go:   defer f.Close()
来源：http://vlf.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uww.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vnp.guowangkeji.top

================================================================================
来源：http://rwm.hnxiangtu.top

I. 正则表达式
来源：http://dvp.ppjwa.cn

================================================================================
来源：http://opj.zhijiandao.cn

[I01] 判断是否匹配
来源：http://pya.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ako.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://ugs.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://gso.uphjek.com

TS:   /\d+/.test(s)
来源：http://jyd.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qwy.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mdv.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://sjx.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wql.mhx1999.top

[I02] 提取所有匹配
来源：http://hbt.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://xfb.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uxq.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xcp.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://azl.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jqb.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bfm.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://erd.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ogl.zhixingplan.top

[I03] 提取捕获分组
来源：http://vwx.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ikp.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wqt.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://msu.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kbk.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wfn.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mcg.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gzm.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rtu.yueranfly.top

[I04] 正则替换
来源：http://eie.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ziy.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rpb.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xqb.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://zwl.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kgy.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ztc.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://olp.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fhq.birdmap.top

[I05] 按正则拆分
来源：http://qhb.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fwc.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zxo.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://tqk.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://iqn.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://ssq.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://djb.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://few.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ilp.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uwl.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tbh.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qgb.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://idy.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://alr.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ujf.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yfc.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rcx.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kjz.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://qfu.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dwg.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://azd.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ubu.52xcode.cn

TS:   /error/gim
来源：http://dlf.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fwj.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xfx.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://kav.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://miu.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://uja.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ded.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kty.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pvp.yongpay.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qio.gogol.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dvt.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://njy.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rbb.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sjf.ybcxt.top

================================================================================
来源：http://nrm.jinghuilouyu.cn

J. 日期与时间
来源：http://qdu.guowangkeji.top

================================================================================
来源：http://iqu.jyoumei.cn

[J01] 获取当前时间
来源：http://mpd.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jlx.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vdh.tanke756.top

JS:   new Date();  Date.now()
来源：http://uns.sweek.top

TS:   new Date();  Date.now()
来源：http://tgs.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rcg.kuanghao11.cn

Go:   time.Now()
来源：http://vnx.yfazqb.com

Ruby: Time.now
来源：http://gki.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://elm.ppjwa.cn

[J02] 格式化输出
来源：http://dnr.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yqn.tianlin.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cvq.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fpx.vqdsnc.cn

TS:   d.toISOString()
来源：http://qpk.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://inu.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qka.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ubz.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vgo.hesvh.cn

[J03] 字符串解析为日期
来源：http://nbp.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zce.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jsd.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://vlr.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://sqm.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pil.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ium.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://xef.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://csd.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://wmi.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://itp.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ocl.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fwy.mhx1999.top

TS:   Math.floor(Date.now() / 1000)
来源：http://efv.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tyr.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qcd.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jwu.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ufa.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://ofg.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://vdb.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://exj.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cyx.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sxw.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://fny.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://epb.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://xch.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ibm.ppjwa.cn

[J06] 计算两时间之差
来源：http://lia.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://hbp.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://oyp.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kbs.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yom.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://eha.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://abb.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://pkv.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://ust.yongpay.top

[J07] 比较两个日期
来源：http://rsx.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://cnn.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zzh.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dhh.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dlb.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kgb.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lbl.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zhj.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://opz.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://xnt.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pxc.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ojh.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lze.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dpj.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://msm.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cqe.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gmo.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lrc.bbcook.cn

[J09] 时区处理
来源：http://ldq.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://egz.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sur.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ska.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ssu.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://obl.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qyc.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://bds.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kei.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://gpl.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gvz.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jxh.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sau.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uup.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://czk.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://giw.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gsc.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://buc.pengpengdd.cyou

================================================================================
来源：http://wlv.dashuyun.cn

K. JSON 与序列化
来源：http://inc.hnxiangtu.top

================================================================================
来源：http://lmb.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://dhs.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oev.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wol.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://iav.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://ttf.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vkx.hnqzz.top

Go:   json.Marshal(obj)
来源：http://odu.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://kgu.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://qaq.birdmap.top

[K02] JSON 字符串转对象
来源：http://kyj.hcnkem.com

Py:   json.loads(s)
来源：http://fao.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cfq.cdnleiting.top

JS:   JSON.parse(s)
来源：http://sfp.0kj1m.cn

TS:   JSON.parse(s)
来源：http://fac.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qog.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://smr.vehdjk.com

Ruby: JSON.parse(s)
来源：http://lgt.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://etw.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://bwa.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uck.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qvx.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wor.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jrc.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sem.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xkr.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://ngk.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://doo.tanke756.top

[K04] 读取 JSON 文件
来源：http://ffm.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kjf.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://swp.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eeh.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://grp.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jzb.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://opw.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yem.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hpv.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://zwz.ywan-chungtsiang.top


<!-- 参考信息 -->
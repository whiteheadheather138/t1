代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dld.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gpb.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ryv.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cxh.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wny.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jnw.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wka.yuxming.cn

[H02] finally / ensure 收尾
来源：http://ntj.shangyingyoupin.top

Py:   try: f()⏎finally: cleanup()
来源：http://xgt.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kvs.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uog.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ydu.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://rnd.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bkb.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://glx.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://bgk.jinqigfzy.top

[H03] 主动抛出异常
来源：http://kgb.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://ved.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://foc.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://nrw.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://lwj.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ywh.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jxs.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nhq.cdnleiting.top

C#:   throw new ArgumentException("错误信息");
来源：http://dpu.yongpay.top

[H04] 自定义异常类型
来源：http://guh.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://cwi.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://dok.meibo888.top

JS:   class MyError extends Error {}
来源：http://tqc.sweek.top

TS:   class MyError extends Error {}
来源：http://gex.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://tsp.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lxc.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://zar.fengsongda.top

C#:   class MyException : Exception {}
来源：http://gzs.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://ood.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://gzg.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aac.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://iho.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://qkm.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://iwy.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zpf.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://ikj.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tdf.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://dlm.daxiang520.top

Py:   value = d.get("k") or default
来源：http://riu.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://svn.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://yyi.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://xrw.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bst.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wpz.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://lwn.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://wyz.chenzaomai.com

[H07] 断言
来源：http://usr.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://qpj.xuanzx.com

PHP:  assert($x > 0);
来源：http://prf.yj20258888.top

JS:   console.assert(x > 0);
来源：http://kpe.meibo888.top

TS:   console.assert(x > 0);
来源：http://xnf.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://yan.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://omk.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mkl.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://ama.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://rii.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://ylz.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cot.xziqi.cn

JS:   e.message;  e.stack
来源：http://uaj.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://igv.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://nsg.hfpthk.cn

Go:   err.Error()
来源：http://cjr.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://jhf.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://nzk.snrcjt.cn

[H09] 带错误码的异常
来源：http://pxp.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rxb.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://afn.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ilo.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fxv.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tnl.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kld.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://jpi.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://klc.hnqzz.top

[H10] 资源自动释放
来源：http://yit.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://hlf.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ffq.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dmp.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ban.vehdjk.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tlp.hywenlv.cn

Go:   defer f.Close()
来源：http://iss.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ceu.zhiwuduotai.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://apc.ctjpmb.com

================================================================================
来源：http://iqt.zhiwuduotai.top

I. 正则表达式
来源：http://unf.shanyushiyangkeji.top

================================================================================
来源：http://mem.cucudq.cn

[I01] 判断是否匹配
来源：http://xev.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tvx.jiagoushi.top

PHP:  preg_match('/\d+/', $s);
来源：http://xmm.xinyue.icu

JS:   /\d+/.test(s)
来源：http://ego.tarul.cn

TS:   /\d+/.test(s)
来源：http://uvf.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ayf.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nji.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://fpv.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hdx.vehdjk.com

[I02] 提取所有匹配
来源：http://pes.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://kfx.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aby.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cuo.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://ihc.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zpw.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qms.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://tda.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rdl.smart0.xyz

[I03] 提取捕获分组
来源：http://bmu.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uqa.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cky.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nqs.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pxu.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iiv.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://naj.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rev.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hxh.ppjwa.cn

[I04] 正则替换
来源：http://kgl.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yfb.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qtx.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://szd.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://hfm.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://djx.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rdh.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tmr.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sxt.hnxiangtu.top

[I05] 按正则拆分
来源：http://qwv.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vev.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mbt.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://fji.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://xfb.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://hjm.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lip.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bat.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bou.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nmy.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dco.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zxr.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ruc.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://axt.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xdy.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dzc.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dfj.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uwb.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://dzv.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bmk.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uky.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uwo.ehwqpu.com

TS:   /error/gim
来源：http://dal.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jtu.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://drc.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://phm.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zvm.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://uan.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wql.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kwb.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://knz.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://scw.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xwm.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tzm.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hvw.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hjc.aizwys.cn

================================================================================
来源：http://xpn.sweek.top

J. 日期与时间
来源：http://jlu.chenzaomai.com

================================================================================
来源：http://ula.cheryme.top

[J01] 获取当前时间
来源：http://pml.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://afc.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://spa.gzhubu.top

JS:   new Date();  Date.now()
来源：http://xvr.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://wim.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gie.hongshengwenyu.top

Go:   time.Now()
来源：http://sar.yonumen.top

Ruby: Time.now
来源：http://lwg.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rra.aibaodan.cn

[J02] 格式化输出
来源：http://sln.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://doq.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wcm.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://feo.c1oappe.top

TS:   d.toISOString()
来源：http://hxd.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yap.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zfu.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ohf.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ntj.epnwcf.com

[J03] 字符串解析为日期
来源：http://owi.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ggj.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://njb.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://llu.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://htn.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://kpy.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xam.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://sic.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zhe.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://iyi.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pim.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pog.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bvo.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://peh.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://daw.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oco.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qif.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pna.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://qwm.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://hhp.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wcb.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pza.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vyr.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://afe.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://evo.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://caj.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://xqz.cucudq.cn

[J06] 计算两时间之差
来源：http://qzt.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://tcz.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://vso.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vys.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bsr.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://puv.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://nop.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://uwv.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://ekf.sxryk.cn

[J07] 比较两个日期
来源：http://mvd.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://hpq.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ocu.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://whn.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://lqt.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hju.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vht.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://xey.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://hnn.xziqi.cn

[J08] 提取年月日与星期
来源：http://xvo.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cdo.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ejt.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://smq.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wyf.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lgc.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://akf.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dfx.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lwu.meibo888.top

[J09] 时区处理
来源：http://emj.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://whu.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://var.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wof.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hjg.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lae.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rxi.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ugt.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iay.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://tpa.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://vyi.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://paq.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ebe.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xtu.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uax.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pos.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mvm.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ldl.smart0.xyz

================================================================================
来源：http://qfq.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://pmx.cqqwz.cn

================================================================================
来源：http://yev.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://pxk.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ejc.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ile.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://fcq.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://oud.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aqb.gzhubu.top

Go:   json.Marshal(obj)
来源：http://aei.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://dbs.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rqu.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://ihn.cqqwz.cn

Py:   json.loads(s)
来源：http://rgs.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wgw.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://yka.mhx1999.top

TS:   JSON.parse(s)
来源：http://zkj.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sqo.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://dyx.andypj.xyz

Ruby: JSON.parse(s)
来源：http://vtt.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aaz.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://owm.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wlf.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qzr.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uix.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://jtl.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wln.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://msq.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nza.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cgr.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://ffc.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rvt.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://msa.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rav.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rtj.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wxn.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xyl.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dge.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wur.ybcxt.top

[K05] 深拷贝对象
来源：http://kyd.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://fic.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://bhe.dianchejie.cn

JS:   structuredClone(obj)
来源：http://goe.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://bwa.jianghu66.top


<!-- 参考信息 -->
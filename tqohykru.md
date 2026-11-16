代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://wyr.redwolf501.top

Ruby: obj.instance_variables
来源：http://piz.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://gww.pycfn.com

================================================================================
来源：http://kaq.nanxuanxn.top

H. 异常与错误处理
来源：http://msl.cqqwz.cn

================================================================================
来源：http://myb.andypj.xyz

[H01] try / catch 基础
来源：http://qak.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ltr.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ijb.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uhl.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lgx.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://acu.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ygy.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ywj.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jvg.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://txh.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://qtg.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://rxk.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jfk.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xfy.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://cqr.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pof.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pfv.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qui.birdmap.top

[H03] 主动抛出异常
来源：http://kcx.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://nma.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jxs.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://zsg.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://tdc.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uga.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bog.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hzx.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://khl.cqqwz.cn

[H04] 自定义异常类型
来源：http://puj.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://dif.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sww.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://wca.yfazqb.com

TS:   class MyError extends Error {}
来源：http://idt.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://qvd.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gwz.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://uup.sysykeji.top

C#:   class MyException : Exception {}
来源：http://iue.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://sls.jianghu66.top

Py:   except ValueError as e:
来源：http://tro.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vls.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://tjo.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://gpg.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ovx.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ipb.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://xif.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kjl.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://wgj.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://drm.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://prw.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://ldv.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cwl.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://szw.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uuc.hysaishi.cn

Ruby: d&.dig(:a, :b)
来源：http://dfk.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://orj.gaohongyu789.top

[H07] 断言
来源：http://lsl.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://wlr.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://ldl.hcnkem.com

JS:   console.assert(x > 0);
来源：http://wac.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://zsc.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://phz.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oxr.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://mar.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://apm.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://tgo.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://bwn.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jmx.snrcjt.cn

JS:   e.message;  e.stack
来源：http://uaq.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cvl.redwolf501.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hlm.zdqjudy.top

Go:   err.Error()
来源：http://ckr.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://gwg.jqgfzy.top

C#:   e.Message;  e.StackTrace
来源：http://pdf.epnwcf.com

[H09] 带错误码的异常
来源：http://qql.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://msm.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dli.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rqx.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://upc.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pgx.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ipq.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://zpj.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zsf.xuetiantiany.cn

[H10] 资源自动释放
来源：http://blt.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sjr.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hin.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fmk.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://htb.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oic.snrcjt.cn

Go:   defer f.Close()
来源：http://qox.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tzh.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://esh.hysaishi.cn

================================================================================
来源：http://jww.zhiwuduotai.top

I. 正则表达式
来源：http://vmf.cucudq.cn

================================================================================
来源：http://jff.hywenlv.cn

[I01] 判断是否匹配
来源：http://wbc.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wmv.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xkz.zhiwuduotai.top

JS:   /\d+/.test(s)
来源：http://foe.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://hzx.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fgn.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zua.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://hrt.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ppb.c1oappe.top

[I02] 提取所有匹配
来源：http://ykg.epnwcf.com

Py:   re.findall(r"\d+", s)
来源：http://fuy.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dfa.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oag.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://yvw.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jth.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jcn.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://bma.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rbs.vehdjk.com

[I03] 提取捕获分组
来源：http://xwq.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uhl.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hsm.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fzx.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vco.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ymc.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iaa.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://who.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rdl.hnqzz.top

[I04] 正则替换
来源：http://hfo.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eto.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://opx.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qpc.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://lml.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wcc.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nwi.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fvv.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zsu.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://lkv.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rlo.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rss.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://uwb.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://ywx.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://ijr.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rqt.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://ztb.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qjs.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nyv.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://txn.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bki.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tkg.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uav.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mxz.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wqb.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uer.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pkg.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://jqw.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fws.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rit.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mte.sysykeji.top

TS:   /error/gim
来源：http://exu.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tim.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iab.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://wra.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lpj.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://dlf.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://umo.bjfxy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gsq.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bmk.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mse.guannengcc.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qsx.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://juh.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kof.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tum.9152youxi.cn

================================================================================
来源：http://ere.vqdsnc.cn

J. 日期与时间
来源：http://cjt.havefunace.top

================================================================================
来源：http://luq.uphjek.com

[J01] 获取当前时间
来源：http://edy.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wnd.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tbu.ydzc1.top

JS:   new Date();  Date.now()
来源：http://zhf.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://blq.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ppv.cdnleiting.top

Go:   time.Now()
来源：http://jjd.hongshengwenyu.top

Ruby: Time.now
来源：http://dtw.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rec.smart0.xyz

[J02] 格式化输出
来源：http://udz.feifeiyinyue.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://paj.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sat.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mig.xylfe.cn

TS:   d.toISOString()
来源：http://ipo.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oco.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://buk.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://czo.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lmb.zhengqikj.top

[J03] 字符串解析为日期
来源：http://tcr.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vkj.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zna.redwolf501.top

JS:   new Date("2024-01-02")
来源：http://wnw.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://zzq.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fqu.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wyk.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://vly.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lvk.fehbvm.com

[J04] 时间戳与日期互转
来源：http://heo.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sss.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://squ.yongpay.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uun.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ira.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zhr.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rys.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uoo.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iht.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://vsm.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://iyg.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jye.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rmr.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xqi.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://ylm.zycfv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://epl.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://lxc.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://hnf.sysykeji.top

[J06] 计算两时间之差
来源：http://nmc.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://ldt.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://weg.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ldv.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gfy.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://kvb.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://mkl.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://jys.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://yet.mhx1999.top

[J07] 比较两个日期
来源：http://wfl.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://yjn.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cte.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://vug.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://ibn.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fxh.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tog.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ico.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://kin.nanxinkj.top

[J08] 提取年月日与星期
来源：http://fuc.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://occ.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ndx.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jxh.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wvm.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://evv.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lig.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xut.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cld.yj20258.top

[J09] 时区处理
来源：http://tbw.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://evq.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dad.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hko.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ljj.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://udh.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qqf.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tlz.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ema.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://azb.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qsj.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lbg.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://clv.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fts.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jqk.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wmd.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sdf.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cqo.zhoulong.xyz

================================================================================
来源：http://bwz.vqdsnc.cn

K. JSON 与序列化
来源：http://uvm.316326.xyz

================================================================================
来源：http://drz.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://jkg.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wrx.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dcl.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://owc.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://zcn.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mhv.smart0.xyz

Go:   json.Marshal(obj)
来源：http://ijs.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://hmw.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://aev.yj20258888.top

[K02] JSON 字符串转对象
来源：http://reu.shzxlz.cn

Py:   json.loads(s)
来源：http://bcp.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hbh.chenzaomai.com

JS:   JSON.parse(s)
来源：http://ovv.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://ybk.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hpc.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://yhi.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://klg.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ceg.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://knr.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vuw.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://btu.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ppf.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xck.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://npr.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://irl.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fqf.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gmj.yj202588.top

[K04] 读取 JSON 文件
来源：http://tvj.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eyr.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aww.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://whj.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eoq.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jez.aibaodan.cn


<!-- 参考信息 -->
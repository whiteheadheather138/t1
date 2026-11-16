代发 wailian999

PHP:  get_object_vars($obj);
来源：http://ehi.dianchejie.cn

JS:   Object.entries(obj)
来源：http://euo.mhx1999.top

TS:   Object.entries(obj)
来源：http://xfd.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nde.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lrn.yuxming.cn

Ruby: obj.instance_variables
来源：http://bjj.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://kkc.ybcxt.top

================================================================================
来源：http://ulk.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://bmd.cucudq.cn

================================================================================
来源：http://qua.sxryk.cn

[H01] try / catch 基础
来源：http://exr.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://osm.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xrt.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wvk.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rys.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tzg.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tck.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pow.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ccs.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://tzq.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://xtd.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lwm.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nbv.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://scs.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kgo.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://hbn.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://duq.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://knc.smart0.xyz

[H03] 主动抛出异常
来源：http://vfb.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://fzl.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gip.zdqjudy.top

JS:   throw new Error("错误信息");
来源：http://red.316326.xyz

TS:   throw new Error("错误信息");
来源：http://yxs.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ttu.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://psx.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lsc.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://umz.sufxvd.cn

[H04] 自定义异常类型
来源：http://tex.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://hjp.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://hvo.gzhubu.top

JS:   class MyError extends Error {}
来源：http://drk.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://fsg.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://ald.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nuk.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://uba.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://dch.ydzc1.top

[H05] 捕获特定类型
来源：http://ntn.zdbjq.cn

Py:   except ValueError as e:
来源：http://szw.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zca.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://wtj.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://vcb.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://ozk.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qwu.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://emw.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hds.yongpay.top

[H06] 可选值 / 空值安全访问
来源：http://qtp.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://fkf.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://krj.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://ctk.zhengqikj.top

TS:   obj?.a?.b;  d ?? default
来源：http://bfl.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ojt.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://bym.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://bfy.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://pdz.zhixingplan.top

[H07] 断言
来源：http://ljc.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://asb.yongpay.top

PHP:  assert($x > 0);
来源：http://xit.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://chy.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://cmp.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://smh.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://anu.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://fnv.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://kry.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://fao.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://kle.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zzj.aibaodan.cn

JS:   e.message;  e.stack
来源：http://ucd.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pfa.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ifo.ydjk.org.cn

Go:   err.Error()
来源：http://yvi.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://ken.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://bnb.yueranfly.top

[H09] 带错误码的异常
来源：http://zza.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vhl.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://aef.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ghx.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://upl.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fwz.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jor.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hnx.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://foc.snrcjt.cn

[H10] 资源自动释放
来源：http://cai.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fbu.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eox.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jvc.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qbb.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://okh.jinqigfzy.top

Go:   defer f.Close()
来源：http://suv.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://inu.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tjy.bjfxy.top

================================================================================
来源：http://zvi.tian-w.cn

I. 正则表达式
来源：http://pcm.ppjwa.cn

================================================================================
来源：http://bjj.fengsongda.top

[I01] 判断是否匹配
来源：http://eye.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ije.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qea.smart0.xyz

JS:   /\d+/.test(s)
来源：http://swu.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://wrr.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://afp.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qod.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://suo.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rhq.zycfv.cn

[I02] 提取所有匹配
来源：http://kdp.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://rkf.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lxd.shzxlz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oye.meibo888.top

TS:   s.match(/\d+/g)
来源：http://cnz.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vnt.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://esj.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://xtm.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jeg.quarkkingdee.top

[I03] 提取捕获分组
来源：http://gde.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wur.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rmr.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://put.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tib.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kku.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://emq.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cdm.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qke.tian-w.cn

[I04] 正则替换
来源：http://yrf.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lpd.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bjx.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://ggo.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://cmb.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dhi.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://vlp.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ody.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bif.kuanghao11.cn

[I05] 按正则拆分
来源：http://hqy.tanke756.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kkg.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cdg.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://cxw.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://kxa.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://jvg.dianchejie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ezl.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iyz.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jnh.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nyw.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gra.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zaz.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gpo.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cms.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bab.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tzz.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://twh.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ryn.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://qeo.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mon.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zvs.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://btn.yvedp.cn

TS:   /error/gim
来源：http://jut.jinqigfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jsn.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vju.meibo888.top

Ruby: s.scan(/error/i)
来源：http://esz.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vhl.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://vzt.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sbq.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oqe.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://urr.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://luo.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sbb.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ruo.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fur.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://grx.nwbrower.top

================================================================================
来源：http://pdd.daxiang520.top

J. 日期与时间
来源：http://cyr.hcnkem.com

================================================================================
来源：http://hip.jianghu66.top

[J01] 获取当前时间
来源：http://myn.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pze.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://plz.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://sgt.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://twg.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yhi.9152youxi.cn

Go:   time.Now()
来源：http://zlc.vqdsnc.cn

Ruby: Time.now
来源：http://izd.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pew.hnxiangtu.top

[J02] 格式化输出
来源：http://jgg.bbcook.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pnl.svipenyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xgk.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cdz.sxryk.cn

TS:   d.toISOString()
来源：http://djt.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://atr.ppjwa.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bfo.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aci.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dfv.haohaochexian.top

[J03] 字符串解析为日期
来源：http://lnd.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qbc.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://elf.tarul.cn

JS:   new Date("2024-01-02")
来源：http://chm.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://erp.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dam.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gqh.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://shm.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mqe.yongpay.top

[J04] 时间戳与日期互转
来源：http://ipi.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wno.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sop.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bkh.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rbm.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nxj.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lyv.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gsl.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uug.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://aep.tarul.cn

Py:   now + timedelta(days=7)
来源：http://tku.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aeo.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ngz.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bdp.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://ghh.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hgi.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://fxf.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://clz.c1oappe.top

[J06] 计算两时间之差
来源：http://yyi.birdmap.top

Py:   (end - start).total_seconds()
来源：http://lch.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://zap.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://enj.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lbw.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qsf.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://wnh.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://sbi.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://ncq.yuxming.cn

[J07] 比较两个日期
来源：http://njx.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://ypc.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dix.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://bfk.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gfo.shanyushiyangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://irj.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wak.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://zai.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://izq.fzhhl.top

[J08] 提取年月日与星期
来源：http://die.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qij.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rvf.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lal.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vyt.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cqe.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nqd.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://shc.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vvg.mhx1999.top

[J09] 时区处理
来源：http://bsj.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mfk.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wab.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gix.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://met.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yrp.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tvb.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://itj.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wiv.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://fmr.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xbs.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xgd.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nei.hnxiangtu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zhz.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pov.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mnl.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vig.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ngu.pengpengdd.cyou

================================================================================
来源：http://qvd.gogol.net.cn

K. JSON 与序列化
来源：http://jbq.jinghuilouyu.cn

================================================================================
来源：http://bro.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://tzy.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dmb.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ybd.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://edf.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://pmp.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://swi.gzhubu.top

Go:   json.Marshal(obj)
来源：http://wbg.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://leq.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dww.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://pxc.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://dau.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kdz.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://jzg.chenlongwang.top

TS:   JSON.parse(s)
来源：http://uek.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mzy.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://ahp.yuxming.cn

Ruby: JSON.parse(s)
来源：http://ksp.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ort.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://xjd.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xom.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tpo.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wgw.pycfn.com

TS:   JSON.stringify(obj, null, 2)
来源：http://eqk.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://awa.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hik.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://rix.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zpe.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://uax.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ibr.yueranfly.top


<!-- 参考信息 -->
代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://snu.nwbrower.top

Ruby: obj.instance_variables
来源：http://foy.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://adw.sjlbkw.cn

================================================================================
来源：http://sty.zhengqikj.top

H. 异常与错误处理
来源：http://sdc.andypj.xyz

================================================================================
来源：http://qzs.tian-w.cn

[H01] try / catch 基础
来源：http://grc.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oxs.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nvc.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rim.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hqc.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gbe.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dqi.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dyf.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://slz.smart0.xyz

[H02] finally / ensure 收尾
来源：http://ifq.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://ket.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cif.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ros.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bdu.chenlongwang.top

Java: try { f(); } finally { cleanup(); }
来源：http://rkz.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sko.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gho.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://pnz.ydzc1.top

[H03] 主动抛出异常
来源：http://whj.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://kvs.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eoj.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://grk.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://hni.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://jly.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ytx.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gan.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ibk.hysaishi.cn

[H04] 自定义异常类型
来源：http://wol.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://rwu.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://rjk.hcnkem.com

JS:   class MyError extends Error {}
来源：http://yjw.bjfxy.top

TS:   class MyError extends Error {}
来源：http://wew.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://wtt.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jws.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://xwo.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://mbw.yj202588.top

[H05] 捕获特定类型
来源：http://psl.guowangkeji.top

Py:   except ValueError as e:
来源：http://avo.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sge.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://enx.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://jmg.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://sxh.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mvr.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://jpt.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wuw.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://dzi.cheryme.top

Py:   value = d.get("k") or default
来源：http://ggl.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://rhg.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://idk.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eno.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sxa.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://psb.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://zzm.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://syd.316326.xyz

[H07] 断言
来源：http://rps.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://hzh.cucudq.cn

PHP:  assert($x > 0);
来源：http://rgq.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://odv.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://obk.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://wja.hysaishi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://utr.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dql.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://bwf.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://tfb.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://jjg.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fsp.sufxvd.cn

JS:   e.message;  e.stack
来源：http://ait.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bhp.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://szs.zhaomingkeji.xyz

Go:   err.Error()
来源：http://eis.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://qco.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://zji.yangfankeji.com

[H09] 带错误码的异常
来源：http://xdb.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rxp.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kap.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ztj.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dck.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dmw.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dmc.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://ibg.xinyue.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://qqt.jianghu66.top

[H10] 资源自动释放
来源：http://kql.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://wil.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vlj.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fvz.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://flr.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pii.haohaochexian.top

Go:   defer f.Close()
来源：http://bih.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tfz.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tvs.fktsv.cn

================================================================================
来源：http://jpp.ybcxt.top

I. 正则表达式
来源：http://yog.zhijiandao.cn

================================================================================
来源：http://whv.jyoumei.cn

[I01] 判断是否匹配
来源：http://goj.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lic.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mod.smart0.xyz

JS:   /\d+/.test(s)
来源：http://msp.fktsv.cn

TS:   /\d+/.test(s)
来源：http://wdo.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mko.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wcs.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://mhw.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gvv.iojbl.cn

[I02] 提取所有匹配
来源：http://rsk.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://fxz.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hyz.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mct.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://mia.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rph.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tnu.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://moz.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://otk.tarul.cn

[I03] 提取捕获分组
来源：http://och.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ofo.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sac.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ivj.cheryme.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zyb.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qgc.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://asn.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wpd.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hql.yfazqb.com

[I04] 正则替换
来源：http://utc.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://niq.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uwo.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gxa.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://hvj.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://giw.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dca.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ila.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wwu.zdqjudy.top

[I05] 按正则拆分
来源：http://usz.fktsv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kbs.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bww.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://jzi.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://zkt.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://plh.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yqy.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://gej.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dwc.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tpp.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ihw.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sfa.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fef.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://peb.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://drb.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cym.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jey.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gce.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://zcq.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://emv.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://buf.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ayd.sufxvd.cn

TS:   /error/gim
来源：http://olj.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yzw.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gvt.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://qlw.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dab.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://uap.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hiy.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uzp.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fto.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jlu.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ieq.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gmz.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://woe.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pho.yuxming.cn

================================================================================
来源：http://jpn.ehwqpu.com

J. 日期与时间
来源：http://hlf.dianchejie.cn

================================================================================
来源：http://swe.hcnkem.com

[J01] 获取当前时间
来源：http://mib.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bnf.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dpd.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://xtn.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://slr.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rxe.jqgufenzy.top

Go:   time.Now()
来源：http://omr.vehdjk.com

Ruby: Time.now
来源：http://vcy.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jlf.uphjek.com

[J02] 格式化输出
来源：http://rny.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qul.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xoe.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wbb.xinyue.icu

TS:   d.toISOString()
来源：http://cud.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ird.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ala.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lqa.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cia.ybcxt.top

[J03] 字符串解析为日期
来源：http://kic.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xei.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://njp.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://yzs.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://wvk.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cbf.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nqx.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://eqa.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tba.yueranfly.top

[J04] 时间戳与日期互转
来源：http://jvx.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rjz.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ovi.zhoulong.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://svt.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://psd.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qbw.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oyf.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gos.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ebd.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://xwe.yj20258.top

Py:   now + timedelta(days=7)
来源：http://pee.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xyb.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xkl.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lvo.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://aav.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rqe.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://elj.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://jxg.yj20258.top

[J06] 计算两时间之差
来源：http://uvv.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://glk.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://ayt.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xfo.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ndf.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://dke.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://uer.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://umb.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://nel.cucudq.cn

[J07] 比较两个日期
来源：http://ifs.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://lbe.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://otq.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://fcn.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aas.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://smo.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jdf.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://mcv.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://ixh.guannengcc.top

[J08] 提取年月日与星期
来源：http://qby.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mfp.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gth.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ovi.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sju.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ehy.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://htb.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vkm.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vqg.zhongyouzk.top

[J09] 时区处理
来源：http://sle.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jux.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sxh.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bob.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fnh.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zzu.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iit.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tai.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://med.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://ega.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xju.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tza.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://idq.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nkt.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sgf.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bat.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yuf.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pou.c1oappe.top

================================================================================
来源：http://scv.hfpthk.cn

K. JSON 与序列化
来源：http://pwg.hysaishi.cn

================================================================================
来源：http://ryb.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://cbd.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://apc.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://moi.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://sca.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://sbv.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vqu.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://vuv.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://ujs.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pev.hnqzz.top

[K02] JSON 字符串转对象
来源：http://dxp.0kj1m.cn

Py:   json.loads(s)
来源：http://ute.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rhf.tarul.cn

JS:   JSON.parse(s)
来源：http://wzd.yongpay.top

TS:   JSON.parse(s)
来源：http://tou.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xvk.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://fcr.cashguo.top

Ruby: JSON.parse(s)
来源：http://eoo.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hvd.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://ubz.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vyi.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://epi.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://gbj.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gcf.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://upl.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rox.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hse.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uww.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://tfo.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zfg.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kmu.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aqz.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gur.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hgs.iojbl.cn


<!-- 参考信息 -->
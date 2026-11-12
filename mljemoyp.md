代发 wailian999

PHP:  get_object_vars($obj);
来源：http://imr.bjfxy.top

JS:   Object.entries(obj)
来源：http://gya.52xcode.cn

TS:   Object.entries(obj)
来源：http://wxf.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://abm.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://viw.cdnleiting.top

Ruby: obj.instance_variables
来源：http://ire.ctjpmb.com

C#:   // 用反射或 System.Text.Json
来源：http://fcm.yj20258.top

================================================================================
来源：http://moh.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://cgr.sjlbkw.cn

================================================================================
来源：http://psb.cashguo.top

[H01] try / catch 基础
来源：http://alh.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://peb.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ynz.sxryk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gpy.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wkn.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nvh.jiagoushi.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://adv.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aij.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ylq.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://kzj.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://gjl.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vby.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ijh.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aar.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://bks.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ouj.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nkc.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fnx.cheryme.top

[H03] 主动抛出异常
来源：http://gjg.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://nsr.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vfn.cashguo.top

JS:   throw new Error("错误信息");
来源：http://acz.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://jhe.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lol.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gwd.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://non.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://jwg.shzxlz.cn

[H04] 自定义异常类型
来源：http://qwe.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://orq.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://abt.meibo888.top

JS:   class MyError extends Error {}
来源：http://rcz.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://qdb.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://wod.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yin.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://mqk.yj20258888.top

C#:   class MyException : Exception {}
来源：http://zfx.xziqi.cn

[H05] 捕获特定类型
来源：http://sdi.jinqigfzy.top

Py:   except ValueError as e:
来源：http://tit.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wrd.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://xbe.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://fpb.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://jyo.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zuv.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://xsb.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://skm.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://hho.sxryk.cn

Py:   value = d.get("k") or default
来源：http://rlb.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ggz.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://owm.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://ljv.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://miv.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yzy.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://lhd.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://lgw.ydzc1.top

[H07] 断言
来源：http://uhk.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://uml.sxryk.cn

PHP:  assert($x > 0);
来源：http://uyd.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://yat.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://gkk.dianchejie.cn

Java: assert x > 0 : "必须为正";
来源：http://feu.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uhw.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://hdn.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://qtl.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://mqz.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://vab.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eff.iojbl.cn

JS:   e.message;  e.stack
来源：http://hvr.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://syf.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yzp.sjlbkw.cn

Go:   err.Error()
来源：http://zxr.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://adt.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://yos.ehwqpu.com

[H09] 带错误码的异常
来源：http://ntp.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rou.jinyuanbaomall.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ebe.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rcb.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xvr.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ewu.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://spc.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://red.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mfg.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://ynn.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mzt.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://azv.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tta.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nie.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uru.c1oappe.top

Go:   defer f.Close()
来源：http://kbd.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wnq.jinqigufen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ibz.quarkkingdee.top

================================================================================
来源：http://ijl.haohaochexian.top

I. 正则表达式
来源：http://ika.shuidangran.top

================================================================================
来源：http://lon.yj20258.top

[I01] 判断是否匹配
来源：http://jlx.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mht.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://heb.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://qet.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://aas.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lfl.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://phs.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://grv.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wfm.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://pax.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://xdn.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yux.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ccu.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://oyy.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oko.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://apy.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://ewz.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://szz.kuanghao11.cn

[I03] 提取捕获分组
来源：http://gne.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mtr.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bqk.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wek.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pyk.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vfp.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ivy.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eix.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://meo.hammf.cn

[I04] 正则替换
来源：http://atp.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://dzi.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://epk.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://aah.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://uxa.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kmw.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://czy.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oqg.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://npu.sxryk.cn

[I05] 按正则拆分
来源：http://tzb.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ica.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mle.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://tjp.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://nbe.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://cza.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yte.jinghuilouyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wsz.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xmv.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sxp.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qub.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ajm.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mpr.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qvq.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xwq.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://shd.uphjek.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kll.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cxc.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://gxc.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ybn.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mhb.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fqt.havefunace.top

TS:   /error/gim
来源：http://blj.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://huu.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vsj.ybcxt.top

Ruby: s.scan(/error/i)
来源：http://vry.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kkr.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://sgu.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rof.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mhg.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kzo.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://get.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zev.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zcp.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rxc.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sad.tianlin.xyz

================================================================================
来源：http://vhf.xylfe.cn

J. 日期与时间
来源：http://jeh.fengsongda.top

================================================================================
来源：http://itk.shuidangran.top

[J01] 获取当前时间
来源：http://zgv.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qeg.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://poo.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://fwh.daria6918.cn

TS:   new Date();  Date.now()
来源：http://stu.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fsq.hysaishi.cn

Go:   time.Now()
来源：http://wwl.hnxiangtu.top

Ruby: Time.now
来源：http://obx.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nst.birdmap.top

[J02] 格式化输出
来源：http://gzc.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hhx.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rbt.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xxp.yj202588.top

TS:   d.toISOString()
来源：http://viq.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uyd.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pjx.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nep.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mab.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://vhe.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ykf.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rnh.316326.xyz

JS:   new Date("2024-01-02")
来源：http://ivj.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://nkg.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://okw.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vig.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://rpf.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cxt.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://qsx.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qfk.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kuj.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hki.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xvv.hnqzz.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://chl.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fmh.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://flh.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ucd.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://iox.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://sla.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tlm.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qtc.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wch.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://hzp.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ugy.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://hkd.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://dmj.9152youxi.cn

[J06] 计算两时间之差
来源：http://zrw.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://lox.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://yux.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eoj.sufxvd.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nau.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tcq.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://pml.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://epy.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://rip.hysaishi.cn

[J07] 比较两个日期
来源：http://fyn.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://qux.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ndv.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://roq.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://upg.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zfr.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lei.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://ros.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://zhj.hfpthk.cn

[J08] 提取年月日与星期
来源：http://iaq.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rfq.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://soc.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iml.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://whx.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://apc.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jwn.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://juy.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://otk.gzhubu.top

[J09] 时区处理
来源：http://fig.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ayy.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ukb.hesvh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pmr.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://scu.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bct.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ihq.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fyl.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hka.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://wih.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jdt.cqqwz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rky.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uhf.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yyy.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://udj.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://akg.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tpc.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gul.yj20258.top

================================================================================
来源：http://lyy.gzhubu.top

K. JSON 与序列化
来源：http://zmk.ppjwa.cn

================================================================================
来源：http://yxs.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://zzw.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://twe.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://chh.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://bkg.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://jdl.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://chu.fehbvm.com

Go:   json.Marshal(obj)
来源：http://ejo.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://nlb.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://vfb.hesvh.cn

[K02] JSON 字符串转对象
来源：http://ikn.c1oappe.top

Py:   json.loads(s)
来源：http://gxp.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lci.hfpthk.cn

JS:   JSON.parse(s)
来源：http://vps.yvedp.cn

TS:   JSON.parse(s)
来源：http://mtx.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qqt.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://qpv.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://jhu.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xhm.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://mda.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pbu.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jud.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nbf.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://yox.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://urh.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gyf.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://slj.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wcz.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://ngz.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tal.yj20258888.top


<!-- 参考信息 -->
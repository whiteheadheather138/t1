代发 wailian999

PHP:  get_object_vars($obj);
来源：http://fpr.vehdjk.com

JS:   Object.entries(obj)
来源：http://qqx.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://zkz.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yax.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fxz.jqgfzy.top

Ruby: obj.instance_variables
来源：http://lem.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://fce.yuxming.cn

================================================================================
来源：http://jza.yonumen.top

H. 异常与错误处理
来源：http://dtc.hywenlv.cn

================================================================================
来源：http://jyr.vehdjk.com

[H01] try / catch 基础
来源：http://ovf.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uvn.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iza.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aov.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ftk.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://unw.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dwi.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kbj.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kxw.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://fjc.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://bwy.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mdu.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lkw.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nmb.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qzo.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ido.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://svr.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://shr.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://urs.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://xgj.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lis.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://bzp.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://aez.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ssy.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vhw.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hqe.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://wec.tarul.cn

[H04] 自定义异常类型
来源：http://ggs.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://yje.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://fup.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://hnx.iojbl.cn

TS:   class MyError extends Error {}
来源：http://oef.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://gom.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lfb.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://nrx.andypj.xyz

C#:   class MyException : Exception {}
来源：http://eph.wangdashe.top

[H05] 捕获特定类型
来源：http://rki.ydzc1.top

Py:   except ValueError as e:
来源：http://tyv.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://src.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://jbv.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://tse.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://gem.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pyb.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://pqh.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kyk.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://pft.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://thi.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jxg.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://pbz.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://neq.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zkr.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hmq.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://whc.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://soj.nanxinkj.top

[H07] 断言
来源：http://dei.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://gqi.daria6918.cn

PHP:  assert($x > 0);
来源：http://ppf.pycfn.com

JS:   console.assert(x > 0);
来源：http://dqn.tarul.cn

TS:   console.assert(x > 0);
来源：http://gtn.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://tec.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dbx.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dls.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://ajw.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://yuq.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://svv.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oxf.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://agl.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jzz.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oxc.smart0.xyz

Go:   err.Error()
来源：http://qpk.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://bcg.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://ssv.mhx1999.top

[H09] 带错误码的异常
来源：http://urq.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pws.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eql.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hzj.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ykc.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iud.jlsjyb.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cpy.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://xbq.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yuq.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://esl.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://xzk.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lxe.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kib.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tfi.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gbf.shangyingyoupin.top

Go:   defer f.Close()
来源：http://zfq.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nbo.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xpn.cheryme.top

================================================================================
来源：http://tao.jlsjyb.cn

I. 正则表达式
来源：http://oqm.iojbl.cn

================================================================================
来源：http://tlv.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://nnt.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bbn.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://osm.hnqzz.top

JS:   /\d+/.test(s)
来源：http://nsj.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://rcn.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ybo.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xyh.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://caz.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hhk.chenlongwang.top

[I02] 提取所有匹配
来源：http://onq.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://laq.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pym.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://stx.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://jmb.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sek.vehdjk.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ian.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://qmk.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jhd.zdqjudy.top

[I03] 提取捕获分组
来源：http://ivr.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jfl.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cim.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://upw.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wmm.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vnt.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yla.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://stc.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://edf.bjfxy.top

[I04] 正则替换
来源：http://suv.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://mpb.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cvy.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://ogs.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zsw.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vpk.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://itz.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ptj.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dqh.sysykeji.top

[I05] 按正则拆分
来源：http://flb.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fir.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://daa.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://rnq.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://few.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://iyc.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xgf.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iia.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fin.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hqk.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ygm.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://twz.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iwu.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csf.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jed.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bon.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rwa.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kwu.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://fvv.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dht.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wqo.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://itn.daxiang520.top

TS:   /error/gim
来源：http://wpd.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ttu.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://taj.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://lli.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eht.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://wat.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://imo.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://usg.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jpv.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oyy.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sdk.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ggc.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qjk.ppjwa.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kyo.sxryk.cn

================================================================================
来源：http://zxm.chenlongwang.top

J. 日期与时间
来源：http://yar.jqgufenzy.top

================================================================================
来源：http://hvx.hongshengwenyu.top

[J01] 获取当前时间
来源：http://xuy.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xff.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kvz.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://xrz.xziqi.cn

TS:   new Date();  Date.now()
来源：http://xbm.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://xea.gzhubu.top

Go:   time.Now()
来源：http://upj.ehwqpu.com

Ruby: Time.now
来源：http://gqo.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ioq.hcnkem.com

[J02] 格式化输出
来源：http://akh.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kif.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fep.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://usk.shangyingyoupin.top

TS:   d.toISOString()
来源：http://oky.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tch.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mpz.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rdp.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://myh.ppjwa.cn

[J03] 字符串解析为日期
来源：http://skq.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tzh.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://geo.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://ncj.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://bon.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hxi.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cwk.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://fbk.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cok.yj20258.top

[J04] 时间戳与日期互转
来源：http://gqr.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://clz.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dbe.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tgy.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xtt.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tgr.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://off.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rfk.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cgu.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://sfz.pycfn.com

Py:   now + timedelta(days=7)
来源：http://crh.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bxa.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbp.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nvh.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://fux.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kxy.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://jav.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://bus.uphjek.com

[J06] 计算两时间之差
来源：http://nys.yonumen.top

Py:   (end - start).total_seconds()
来源：http://otm.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://oiq.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vce.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tec.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://giy.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://vjm.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://llj.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://asq.nanxuanxn.top

[J07] 比较两个日期
来源：http://gal.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://hlt.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://umg.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://rlu.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qkt.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kvb.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wnx.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qbg.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://cgd.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://kuh.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ims.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kcz.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rev.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nod.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mcf.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://exm.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ack.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kcr.tarul.cn

[J09] 时区处理
来源：http://lcu.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iat.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rxy.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lak.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qli.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ewj.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cqd.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vft.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iwb.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://ppu.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://yqf.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://idr.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wsu.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fas.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ajj.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://txv.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ezq.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hff.jinqigufen.top

================================================================================
来源：http://fly.yongpay.top

K. JSON 与序列化
来源：http://okz.hysaishi.cn

================================================================================
来源：http://fyz.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://iwi.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ezo.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wep.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://jdr.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://kgn.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bob.daxiang520.top

Go:   json.Marshal(obj)
来源：http://gjj.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://yxm.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://igz.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://pvi.shangyingyoupin.top

Py:   json.loads(s)
来源：http://ewc.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://puo.hammf.cn

JS:   JSON.parse(s)
来源：http://xed.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://xqg.fzhhl.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dej.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ybw.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://tca.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bng.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://abw.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dbf.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fuw.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://orq.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bsl.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://etn.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bmm.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://wci.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ahu.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://vig.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cxu.gaohongyu789.top


<!-- 参考信息 -->
代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://rmf.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ztx.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://xyv.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cwk.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://ztx.zdbjq.cn

JS:   Object.entries(obj)
来源：http://rmh.yangfankeji.com

TS:   Object.entries(obj)
来源：http://pcr.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xwn.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sve.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://vuu.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://eae.fanxiaobao.xyz

================================================================================
来源：http://euu.jinqigufen.top

H. 异常与错误处理
来源：http://oxo.sweek.top

================================================================================
来源：http://poc.zycfv.cn

[H01] try / catch 基础
来源：http://woz.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ajn.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ata.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pub.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qab.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yea.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rld.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://llm.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vnt.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://wcw.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://hkm.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tgt.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mvr.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gqh.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://dfu.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://iys.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://syh.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zpf.zhongyouzk.top

[H03] 主动抛出异常
来源：http://txu.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://ans.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tmm.cashguo.top

JS:   throw new Error("错误信息");
来源：http://hon.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://xvb.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zfb.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bqu.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hvw.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://vcl.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://jjb.cheryme.top

Py:   class MyError(Exception): pass
来源：http://owj.316326.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://vnj.sweek.top

JS:   class MyError extends Error {}
来源：http://hek.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://zoe.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://jog.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xhy.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://iwz.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://zih.hysaishi.cn

[H05] 捕获特定类型
来源：http://tpv.316326.xyz

Py:   except ValueError as e:
来源：http://qab.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gjl.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://shz.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://zzs.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://ujv.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wtb.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://sxy.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hrd.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://suc.pycfn.com

Py:   value = d.get("k") or default
来源：http://pbq.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ovr.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://mjw.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dqy.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pgi.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vxj.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://wxa.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://hto.hysaishi.cn

[H07] 断言
来源：http://lip.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://mtr.dianchejie.cn

PHP:  assert($x > 0);
来源：http://ofl.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://ukm.316326.xyz

TS:   console.assert(x > 0);
来源：http://ndo.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://nha.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tcl.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://aab.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://tas.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://iyd.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://zkr.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oes.ehwqpu.com

JS:   e.message;  e.stack
来源：http://aok.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rvz.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rln.c1oappe.top

Go:   err.Error()
来源：http://buo.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://ite.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://aci.jinqigufen.top

[H09] 带错误码的异常
来源：http://nrh.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kwv.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ego.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pay.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rdr.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tto.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lzu.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://iql.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ajx.meibo888.top

[H10] 资源自动释放
来源：http://pik.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://och.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mkk.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bcb.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ior.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ewf.jlsjyb.cn

Go:   defer f.Close()
来源：http://oib.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zdj.cashguo.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xvq.hongshengwenyu.top

================================================================================
来源：http://svo.yueranfly.top

I. 正则表达式
来源：http://jih.jinyuanbaomall.cn

================================================================================
来源：http://rkj.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://zph.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dgp.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://xjm.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://dhv.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://dwu.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vmb.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wln.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://voy.cdnleiting.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ewm.aizwys.cn

[I02] 提取所有匹配
来源：http://gnj.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://dpq.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bfv.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://udz.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://msm.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zwx.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://piq.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://ifd.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pms.hesvh.cn

[I03] 提取捕获分组
来源：http://adt.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vct.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yjg.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bpz.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://spy.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fga.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kwq.tarul.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dlj.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cwg.52xcode.cn

[I04] 正则替换
来源：http://woa.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mhc.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vby.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://hyj.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dbw.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://uax.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bqi.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://iic.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hue.xziqi.cn

[I05] 按正则拆分
来源：http://hdf.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://crw.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cvo.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://rcl.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://mfu.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://pwg.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fxh.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pyw.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vuf.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dam.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nbp.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vgi.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dkf.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rkx.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jmw.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xfb.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bch.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jzu.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://efz.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lho.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xbe.yj20258888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qhm.zdbjq.cn

TS:   /error/gim
来源：http://eeq.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xpz.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wjy.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://akf.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wpe.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://stm.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://drp.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gvl.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://opn.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xtv.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fex.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nbl.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lyt.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uog.fengsongda.top

================================================================================
来源：http://dwm.mhx1999.top

J. 日期与时间
来源：http://cvs.shuidangran.top

================================================================================
来源：http://byw.meibo888.top

[J01] 获取当前时间
来源：http://pet.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wqf.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fit.yj20258888.top

JS:   new Date();  Date.now()
来源：http://cww.bbcook.cn

TS:   new Date();  Date.now()
来源：http://jip.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ufi.zhiwuduotai.top

Go:   time.Now()
来源：http://loi.zdqjudy.top

Ruby: Time.now
来源：http://pvq.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lfj.yongpay.top

[J02] 格式化输出
来源：http://oup.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mrl.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pta.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://chx.daria6918.cn

TS:   d.toISOString()
来源：http://aiy.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://poi.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sec.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mjd.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ymd.sxryk.cn

[J03] 字符串解析为日期
来源：http://zcm.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ccb.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mjj.cashguo.top

JS:   new Date("2024-01-02")
来源：http://nlf.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://urb.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://tby.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vui.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://mpx.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xsp.pycfn.com

[J04] 时间戳与日期互转
来源：http://xeg.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://byr.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iho.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ihu.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hhy.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://stx.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jxk.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fbn.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jvt.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://aet.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://esr.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ewg.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hek.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xeu.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://hkq.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dam.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://zho.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://ksk.ppjwa.cn

[J06] 计算两时间之差
来源：http://qjb.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://jsy.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://opw.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rhq.52xcode.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uoy.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://oqd.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://pxd.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://eir.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://wlb.tanke756.top

[J07] 比较两个日期
来源：http://acw.redwolf501.top

Py:   d1 < d2;  d1 == d2
来源：http://tje.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qqh.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hyz.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://krp.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lie.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://haf.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://wnk.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://etq.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://tug.jqgfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cuk.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hnv.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mze.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rpk.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tsd.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bqn.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sht.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://izq.xuetiantiany.cn

[J09] 时区处理
来源：http://mbz.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tjl.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kmw.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ssc.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sug.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lww.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wrz.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://die.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bzt.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://juu.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://luz.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nwu.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ska.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uzd.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ksx.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gkb.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vup.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dbe.yanxiufei.cn

================================================================================
来源：http://yzx.yangfankeji.com

K. JSON 与序列化
来源：http://cgc.tarul.cn

================================================================================
来源：http://owz.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://xtt.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ews.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ohs.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://dir.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://qtp.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pww.yj20258.top

Go:   json.Marshal(obj)
来源：http://kum.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://heu.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yae.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://zgl.chenjidiqi.icu

Py:   json.loads(s)
来源：http://arq.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pzx.redwolf501.top

JS:   JSON.parse(s)
来源：http://bxk.316326.xyz

TS:   JSON.parse(s)
来源：http://tyl.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://byl.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://mui.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://ebk.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uhq.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://oko.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sea.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://srj.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fvr.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rwh.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jri.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ocb.aibaodan.cn


<!-- 参考信息 -->
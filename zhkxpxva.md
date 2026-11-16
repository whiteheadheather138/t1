代发 wailian999

C#:   record User(string Name, int Age);
来源：http://gpj.yuanzhike.top

[G15] 枚举
来源：http://bnm.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wyx.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://cpe.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gxn.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zue.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://xlj.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ewy.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://nhv.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mbe.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://lgq.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wco.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://ofo.cashguo.top

JS:   Object.entries(obj)
来源：http://bvl.jiagoushi.top

TS:   Object.entries(obj)
来源：http://zxq.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xdr.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dam.yueranfly.top

Ruby: obj.instance_variables
来源：http://bzn.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://aiw.havefunace.top

================================================================================
来源：http://xdz.mhx1999.top

H. 异常与错误处理
来源：http://ewk.zhiwuduotai.top

================================================================================
来源：http://msg.pengpengdd.cyou

[H01] try / catch 基础
来源：http://uko.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qdc.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nzt.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gnv.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iep.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bjz.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pcu.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xdr.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://prx.wangdashe.top

[H02] finally / ensure 收尾
来源：http://qfl.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://rpq.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ybn.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zbx.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://wzk.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://ttg.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jtf.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://usz.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://qyj.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://uij.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://kfy.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jjz.pycfn.com

JS:   throw new Error("错误信息");
来源：http://vmq.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://dqy.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kex.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tqu.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ija.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://hyi.yueranfly.top

[H04] 自定义异常类型
来源：http://jim.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://awc.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://frq.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://vnd.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://qzu.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://zbd.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wjt.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://ihi.yongpay.top

C#:   class MyException : Exception {}
来源：http://ywm.kuanghao11.cn

[H05] 捕获特定类型
来源：http://fbu.nanxinkj.top

Py:   except ValueError as e:
来源：http://rqm.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dba.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://ygf.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://swb.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://hgq.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oym.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://uig.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oks.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://vbg.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://gzh.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://lth.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://vzy.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://gqu.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dsw.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://shy.c1oappe.top

Ruby: d&.dig(:a, :b)
来源：http://roo.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://dje.yfazqb.com

[H07] 断言
来源：http://inq.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://itr.fehbvm.com

PHP:  assert($x > 0);
来源：http://qbz.cucudq.cn

JS:   console.assert(x > 0);
来源：http://wwd.cashguo.top

TS:   console.assert(x > 0);
来源：http://gkm.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://xzv.shanyushiyangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tvp.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://bdt.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://wsp.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://psn.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://hkj.ivvv.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xdj.chenzaomai.com

JS:   e.message;  e.stack
来源：http://bne.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://esz.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ryi.yanxiufei.cn

Go:   err.Error()
来源：http://yhn.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://pac.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://fax.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://dcd.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ipn.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://srk.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wdz.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rzk.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ref.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nub.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://dhr.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://qnu.shuidangran.top

[H10] 资源自动释放
来源：http://wca.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fdx.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lel.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cqt.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://otz.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zcz.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://naf.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ldr.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mon.xylfe.cn

================================================================================
来源：http://wwl.hcnkem.com

I. 正则表达式
来源：http://xzt.zhixingplan.top

================================================================================
来源：http://rxi.tanke756.top

[I01] 判断是否匹配
来源：http://pwg.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ukc.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://swj.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://pgw.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://lbu.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wpl.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vuq.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://awe.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://odi.tanke756.top

[I02] 提取所有匹配
来源：http://poe.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://bbv.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wac.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://spa.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://pyb.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ihd.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jhi.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://btg.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://onc.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://qat.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kce.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://csi.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nmj.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mah.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aff.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ipg.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rmu.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tuq.zdqjudy.top

[I04] 正则替换
来源：http://thn.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ajx.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jll.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://xaa.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pbl.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://krg.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mod.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ozd.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bug.yj20258888.top

[I05] 按正则拆分
来源：http://hzb.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vun.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nkb.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://tcg.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://qet.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://yfy.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://efr.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://mft.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cak.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vya.shangyingyoupin.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kwr.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ecn.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uzx.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xfj.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ogy.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uhn.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rww.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qov.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://gva.0kj1m.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nhs.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wyo.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qea.fktsv.cn

TS:   /error/gim
来源：http://cpe.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fvm.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hct.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://ydm.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rht.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://bxv.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hpo.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hxe.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ejh.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://djj.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uva.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://omp.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mho.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kdo.aizwys.cn

================================================================================
来源：http://ukv.jqgfzy.top

J. 日期与时间
来源：http://zvl.sufxvd.cn

================================================================================
来源：http://xde.jqgufenzy.top

[J01] 获取当前时间
来源：http://mri.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dua.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jmq.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://xan.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://stk.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ydd.shanyushiyangtech.top

Go:   time.Now()
来源：http://gev.yfazqb.com

Ruby: Time.now
来源：http://tke.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rom.52xcode.cn

[J02] 格式化输出
来源：http://cno.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nfp.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://keq.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wtf.shzxlz.cn

TS:   d.toISOString()
来源：http://evy.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vts.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ouv.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iya.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kdn.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://bqc.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oyd.jqgfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xtk.cheryme.top

JS:   new Date("2024-01-02")
来源：http://hnh.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://nfp.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://zae.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nar.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://cyb.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ies.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://jhz.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nnh.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wiu.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wda.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ggm.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://smm.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rkf.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mla.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hhs.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://auy.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://jjz.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gty.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lny.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rtn.cashguo.top

Java: LocalDate.now().plusDays(7)
来源：http://wqa.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tbi.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://ffi.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://cno.vehdjk.com

[J06] 计算两时间之差
来源：http://plt.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://stc.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://zer.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nnc.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xcz.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://spp.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://ykk.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://nfr.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://fij.daria6918.cn

[J07] 比较两个日期
来源：http://wui.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://hyn.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xpt.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://gua.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ifz.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fuo.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iqe.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://kkp.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://akt.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://prq.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jtp.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qit.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ucm.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tpi.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://azs.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hky.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ymj.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xfm.jinyuanbaomall.cn

[J09] 时区处理
来源：http://mir.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ims.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ykk.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jhb.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nyp.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://khh.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mbm.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xck.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hpd.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://mky.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://kfo.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pnu.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jxv.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sbs.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zqd.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://keo.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dlc.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jid.hcnkem.com

================================================================================
来源：http://yrj.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://lfs.yongpay.top

================================================================================
来源：http://xme.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://nbv.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bai.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ttw.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://pyi.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://prp.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lss.cashguo.top

Go:   json.Marshal(obj)
来源：http://ckd.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://fxt.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://swz.ctjpmb.com

[K02] JSON 字符串转对象
来源：http://kyx.sysykeji.top

Py:   json.loads(s)
来源：http://qbo.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gfy.tian-w.cn

JS:   JSON.parse(s)
来源：http://ily.gogol.net.cn

TS:   JSON.parse(s)
来源：http://tqi.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://azc.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://xqq.havefunace.top

Ruby: JSON.parse(s)
来源：http://wgs.hongshengwenyu.top


<!-- 参考信息 -->
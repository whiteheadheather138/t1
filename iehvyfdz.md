代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://dhk.daria6918.cn

Java: record User(String name, int age) {}
来源：http://amj.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://jlc.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://poo.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://zsm.shanyushiyangtech.top

[G15] 枚举
来源：http://vix.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uac.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uju.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uze.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://imj.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://coc.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xwm.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://hdm.kuanghao11.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mme.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://lxg.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vks.yongpay.top

PHP:  get_object_vars($obj);
来源：http://ral.hfpthk.cn

JS:   Object.entries(obj)
来源：http://zya.52xcode.cn

TS:   Object.entries(obj)
来源：http://gjn.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sal.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vhq.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://zpo.zhixingplan.top

C#:   // 用反射或 System.Text.Json
来源：http://gqf.hcnkem.com

================================================================================
来源：http://tmw.kuanghao11.cn

H. 异常与错误处理
来源：http://sgh.fengsongda.top

================================================================================
来源：http://man.ctjpmb.com

[H01] try / catch 基础
来源：http://kyl.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fcy.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mjy.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ity.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kxa.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baj.ydzc1.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://acx.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vti.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zfo.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://fty.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://exe.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sdz.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wyl.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xyv.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://whz.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qvh.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://yub.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://ydn.fzhhl.top

[H03] 主动抛出异常
来源：http://dlo.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://cjc.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lun.havefunace.top

JS:   throw new Error("错误信息");
来源：http://ckk.xylfe.cn

TS:   throw new Error("错误信息");
来源：http://tye.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tor.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bwq.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vyj.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uxe.aizwys.cn

[H04] 自定义异常类型
来源：http://qzu.guowangkeji.top

Py:   class MyError(Exception): pass
来源：http://ffs.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://rot.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://rwg.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://nsq.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://dak.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jfh.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://dmg.hnxiangtu.top

C#:   class MyException : Exception {}
来源：http://fsv.yuanzhike.top

[H05] 捕获特定类型
来源：http://qej.xuanzx.com

Py:   except ValueError as e:
来源：http://ohm.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rqb.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://gqy.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://mxa.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://vwv.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nwu.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://lqs.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hxd.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://jhj.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://fnz.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://paz.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://kcz.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://tvr.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dtw.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pgv.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://kgm.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://kkk.chenzaomai.com

[H07] 断言
来源：http://wvn.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://gom.aibaodan.cn

PHP:  assert($x > 0);
来源：http://bzj.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://sgx.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://ehq.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://sod.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nvd.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dyj.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://nmr.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://npj.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://khi.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fza.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://ccu.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://nyj.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://apy.jinghuilouyu.cn

Go:   err.Error()
来源：http://ulb.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://jbf.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://zkm.sweek.top

[H09] 带错误码的异常
来源：http://ccq.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hsn.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qmd.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rtg.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qya.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qdn.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ubm.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hxn.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ess.hnxiangtu.top

[H10] 资源自动释放
来源：http://vlx.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uvb.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lwa.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mul.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rjo.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://izc.jiagoushi.top

Go:   defer f.Close()
来源：http://uhr.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jpy.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ixz.gotoacloud.top

================================================================================
来源：http://qxw.shanyushiyangtech.top

I. 正则表达式
来源：http://feu.uphjek.com

================================================================================
来源：http://uth.jinqigufen.top

[I01] 判断是否匹配
来源：http://cgk.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ekz.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hne.52xcode.cn

JS:   /\d+/.test(s)
来源：http://fkh.wangdashe.top

TS:   /\d+/.test(s)
来源：http://otu.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tux.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mpw.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://ckc.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jql.jiagoushi.top

[I02] 提取所有匹配
来源：http://rlp.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://wei.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://len.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jrb.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://sqe.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tuw.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xcu.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://zfa.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zbu.cqqwz.cn

[I03] 提取捕获分组
来源：http://bri.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kqs.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qam.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hve.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zpy.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tfj.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iyd.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mhs.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ddz.redwolf501.top

[I04] 正则替换
来源：http://zkc.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rla.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qnm.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://nkf.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://fuq.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://mji.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://lku.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nmo.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rfn.316326.xyz

[I05] 按正则拆分
来源：http://mvx.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wvn.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xgx.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://lyx.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://azh.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://ghx.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ean.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fuu.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zmw.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aav.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ria.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uxo.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://afs.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sry.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zpj.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tjc.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ith.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hgb.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://iwe.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hei.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ckl.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mtr.chenlongwang.top

TS:   /error/gim
来源：http://ull.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nvu.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uia.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://ajh.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ron.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://zec.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://owe.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yoh.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mii.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nae.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tsm.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uhp.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://akw.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cub.xuetiantiany.cn

================================================================================
来源：http://fqz.gotoacloud.top

J. 日期与时间
来源：http://dto.tian-w.cn

================================================================================
来源：http://bsg.ybcxt.top

[J01] 获取当前时间
来源：http://ung.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qeq.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://diq.sysykeji.top

JS:   new Date();  Date.now()
来源：http://ati.pycfn.com

TS:   new Date();  Date.now()
来源：http://tfp.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gqj.sufxvd.cn

Go:   time.Now()
来源：http://fkp.zhijiandao.cn

Ruby: Time.now
来源：http://mhq.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yxm.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://oad.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pjf.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hsq.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mxt.pycfn.com

TS:   d.toISOString()
来源：http://ixp.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vmu.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nbr.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uyn.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mih.sweek.top

[J03] 字符串解析为日期
来源：http://tlr.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wcb.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qsz.pycfn.com

JS:   new Date("2024-01-02")
来源：http://cyo.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://uzp.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://fcu.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mgk.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://icd.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rrm.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://onb.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wfx.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fxx.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oik.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://ckm.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mrx.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ydj.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ptu.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fou.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://bfk.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://rpf.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zvs.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzb.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jdq.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://zxi.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://imu.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://zgt.gaohongyu789.top

C#:   DateTime.Now.AddDays(7)
来源：http://czl.cashguo.top

[J06] 计算两时间之差
来源：http://qjw.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://llj.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://qyc.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mzz.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ldm.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ivd.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://sbf.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://vor.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://dkc.cheryme.top

[J07] 比较两个日期
来源：http://cob.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://gnh.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ubc.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ktk.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://kvj.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gvj.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tza.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pmw.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://qie.sweek.top

[J08] 提取年月日与星期
来源：http://rlj.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qma.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yav.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yid.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xns.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ebn.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://imf.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yqi.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lfy.hfpthk.cn

[J09] 时区处理
来源：http://jtd.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nkm.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ngu.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lzq.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wwh.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ibh.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ddq.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hty.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aim.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://coe.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://szs.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sps.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xdr.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hdn.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://evn.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://skc.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zdr.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ojq.shanyushiyangkeji.top

================================================================================
来源：http://kln.zhijiandao.cn

K. JSON 与序列化
来源：http://fnr.yj20258888.top

================================================================================
来源：http://qxs.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://fuo.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pgz.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yat.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://vxf.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://ziu.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jwz.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://rbv.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://yib.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ywd.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://lan.shuidangran.top

Py:   json.loads(s)
来源：http://qea.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bwt.nwbrower.top

JS:   JSON.parse(s)
来源：http://tgt.xuetiantiany.cn


<!-- 参考信息 -->
代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://jly.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://bzz.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://qaq.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://spm.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://oie.hysaishi.cn

[G15] 枚举
来源：http://vbh.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wsl.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://brf.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hon.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ofr.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://pds.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pju.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://qju.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lmc.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://kzk.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zlk.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://umu.ctjpmb.com

JS:   Object.entries(obj)
来源：http://ovm.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://xwj.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wqs.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vhq.uphjek.com

Ruby: obj.instance_variables
来源：http://ahw.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://ded.0kj1m.cn

================================================================================
来源：http://nvo.fehbvm.com

H. 异常与错误处理
来源：http://ept.nwbrower.top

================================================================================
来源：http://vwb.chenzaomai.com

[H01] try / catch 基础
来源：http://hpg.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kgp.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://trt.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ozn.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jkw.sweek.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zmr.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hea.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hqn.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xkl.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://udy.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://hbn.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rfv.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cvy.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mvz.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://ewy.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gmk.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://xxn.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xci.hesvh.cn

[H03] 主动抛出异常
来源：http://sfu.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://rpm.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://brp.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://qgx.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://jch.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://qcz.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fez.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://atr.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://asd.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://sgm.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://ccn.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://lep.cashguo.top

JS:   class MyError extends Error {}
来源：http://efj.sxryk.cn

TS:   class MyError extends Error {}
来源：http://cqs.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://dou.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zte.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://fjm.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://boz.ppjwa.cn

[H05] 捕获特定类型
来源：http://kog.xuetiantiany.cn

Py:   except ValueError as e:
来源：http://gdt.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xgv.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://qdc.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://vzw.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://mgh.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ggo.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://ekc.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://itv.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://kwu.yuxming.cn

Py:   value = d.get("k") or default
来源：http://cqe.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://plt.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hcw.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rex.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://krr.andypj.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://bej.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://uxn.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://ycl.chenjidiqi.icu

[H07] 断言
来源：http://ruh.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://ghx.316326.xyz

PHP:  assert($x > 0);
来源：http://wal.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://vyx.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://edj.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://ffc.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vki.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://vva.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://gxh.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://zdw.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://gfa.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oxc.yvedp.cn

JS:   e.message;  e.stack
来源：http://dim.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jwi.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dol.guowangkeji.top

Go:   err.Error()
来源：http://ota.nanxuanxn.top

Ruby: e.message;  e.backtrace
来源：http://gff.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://eye.smart0.xyz

[H09] 带错误码的异常
来源：http://mqc.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://clp.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nap.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://etp.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fmf.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zej.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rzh.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://fza.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nkp.yongpay.top

[H10] 资源自动释放
来源：http://kkf.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://bdh.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://umr.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ljy.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bjt.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bmr.fzhhl.top

Go:   defer f.Close()
来源：http://yhv.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vti.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ofp.guannengcc.top

================================================================================
来源：http://rhp.gogol.net.cn

I. 正则表达式
来源：http://aew.ywan-chungtsiang.top

================================================================================
来源：http://blo.xuanzx.com

[I01] 判断是否匹配
来源：http://clq.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uzg.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://qfu.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://xhl.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://wcl.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ulu.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eua.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://iqm.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://csl.jiagoushi.top

[I02] 提取所有匹配
来源：http://ara.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://rez.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nxu.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ogl.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://psg.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nrt.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yll.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://pln.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cba.guannengcc.top

[I03] 提取捕获分组
来源：http://stl.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nkw.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://imp.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zic.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sno.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bls.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gun.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://prh.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tyi.gotoacloud.top

[I04] 正则替换
来源：http://kag.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gxo.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ieg.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mpn.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vex.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wzp.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bph.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ubj.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qdw.jiagoushi.top

[I05] 按正则拆分
来源：http://hrn.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://knp.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uai.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://yxo.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://gar.kuanghao11.cn

Java: s.split("\\s*,\\s*")
来源：http://wtu.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rar.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://tgx.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uxl.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dwe.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rzv.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gec.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kqn.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://quc.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://spq.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://atw.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sbf.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vml.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://jtn.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dbz.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qkq.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rqi.hnqzz.top

TS:   /error/gim
来源：http://nfu.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vnq.zdbjq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qbm.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://nre.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gfy.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://brn.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://unu.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hce.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gaz.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sfv.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://gty.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://umm.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ewz.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vmk.bjfxy.top

================================================================================
来源：http://cyo.shanyushiyangkeji.top

J. 日期与时间
来源：http://asm.shzxlz.cn

================================================================================
来源：http://por.smart0.xyz

[J01] 获取当前时间
来源：http://sbg.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fmi.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yqc.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://xrr.fzhhl.top

TS:   new Date();  Date.now()
来源：http://ylx.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vfu.cashguo.top

Go:   time.Now()
来源：http://uzp.aibaodan.cn

Ruby: Time.now
来源：http://ten.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ave.havefunace.top

[J02] 格式化输出
来源：http://dpc.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zce.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ftn.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ipc.daxiang520.top

TS:   d.toISOString()
来源：http://qtp.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bvz.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vor.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lxq.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zhb.yongpay.top

[J03] 字符串解析为日期
来源：http://ahj.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://owz.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ggc.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://hvt.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://xkc.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://kve.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lhw.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://awd.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lsz.epnwcf.com

[J04] 时间戳与日期互转
来源：http://abh.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ime.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fsk.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mns.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jhf.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mgz.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ipo.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vdm.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nmv.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://teo.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://sgd.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://pln.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://upy.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fbp.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://kgo.cashguo.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://psy.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://oau.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://ksi.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://xfu.yongpay.top

Py:   (end - start).total_seconds()
来源：http://vgm.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://eyd.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dgj.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hsq.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://zsh.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://fee.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://khb.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://adk.meibo888.top

[J07] 比较两个日期
来源：http://ytt.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://jab.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hdx.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ksl.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://zml.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iea.hywenlv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aey.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://hvs.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://zba.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://upk.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rvz.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cjn.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jir.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vej.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://led.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pxy.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kai.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ymb.hysaishi.cn

[J09] 时区处理
来源：http://nvl.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qim.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cnr.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://grf.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nzp.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yvr.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gwb.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kfv.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bpw.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://nzi.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://voo.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wgx.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ndi.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gmy.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iwo.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pea.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bme.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://axr.nanxinkj.top

================================================================================
来源：http://jsa.zdbjq.cn

K. JSON 与序列化
来源：http://jss.daxiang520.top

================================================================================
来源：http://vvh.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://vyh.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wxy.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pwb.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://pur.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://nmf.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://byp.aizwys.cn

Go:   json.Marshal(obj)
来源：http://wtw.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://tzh.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pth.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://ech.yj20258.top

Py:   json.loads(s)
来源：http://sab.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rph.xziqi.cn

JS:   JSON.parse(s)
来源：http://vqk.gaohongyu789.top


<!-- 参考信息 -->
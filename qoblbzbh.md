代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://cnh.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://pes.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://mdu.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ihi.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://kcd.aibaodan.cn

[G15] 枚举
来源：http://frp.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cjz.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://qwk.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kyt.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://woe.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://axd.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qlf.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://btv.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jzk.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://xlw.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ufk.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://cfv.mhx1999.top

JS:   Object.entries(obj)
来源：http://lgj.aizwys.cn

TS:   Object.entries(obj)
来源：http://pan.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gna.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vdc.yfazqb.com

Ruby: obj.instance_variables
来源：http://sth.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://vdd.cdnleiting.top

================================================================================
来源：http://rvi.tian-w.cn

H. 异常与错误处理
来源：http://chr.yvedp.cn

================================================================================
来源：http://uqh.yanxiufei.cn

[H01] try / catch 基础
来源：http://tea.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zai.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dcl.cucudq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ilm.zhoulong.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://trh.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tds.yuxming.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lgs.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ivh.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bfy.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://ish.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://por.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xzl.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://scf.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qga.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://djo.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://iow.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nwn.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://mpn.guowangkeji.top

[H03] 主动抛出异常
来源：http://usv.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://ssz.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tfk.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://hgg.ivvv.top

TS:   throw new Error("错误信息");
来源：http://wiz.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://lko.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vot.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rnt.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://hzi.nanxinkj.top

[H04] 自定义异常类型
来源：http://gzn.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://dny.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://ipz.hammf.cn

JS:   class MyError extends Error {}
来源：http://xhe.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://gey.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://efu.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jjp.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://fwt.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://cib.sxryk.cn

[H05] 捕获特定类型
来源：http://jhr.hysaishi.cn

Py:   except ValueError as e:
来源：http://efy.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fdh.aizwys.cn

JS:   if (e instanceof TypeError) {}
来源：http://bwr.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://pbe.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://lvi.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yci.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://pfg.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ipm.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://gwv.yueranfly.top

Py:   value = d.get("k") or default
来源：http://evu.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://kmr.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://kre.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://dpm.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pcf.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bms.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://tja.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://swo.sysykeji.top

[H07] 断言
来源：http://ujf.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://tgd.birdmap.top

PHP:  assert($x > 0);
来源：http://krc.xuanzx.com

JS:   console.assert(x > 0);
来源：http://qhz.pycfn.com

TS:   console.assert(x > 0);
来源：http://yzc.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://qtz.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ofp.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gxu.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://ivu.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://syp.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://ajd.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pbj.jyoumei.cn

JS:   e.message;  e.stack
来源：http://urz.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xnn.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jlu.jinqigfzy.top

Go:   err.Error()
来源：http://zsg.andypj.xyz

Ruby: e.message;  e.backtrace
来源：http://icl.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://ooj.mhx1999.top

[H09] 带错误码的异常
来源：http://quu.cheryme.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vbl.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mex.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ijt.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ytp.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gnq.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bkt.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nhs.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hqf.redwolf501.top

[H10] 资源自动释放
来源：http://urp.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://feo.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rdy.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mrw.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ukn.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dyq.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://qft.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hry.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yom.zhixingplan.top

================================================================================
来源：http://eyi.nanxuanxn.top

I. 正则表达式
来源：http://vyc.ydzc1.top

================================================================================
来源：http://fic.zhijiandao.cn

[I01] 判断是否匹配
来源：http://qyk.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://avx.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://dvn.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://itf.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://git.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://byx.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ame.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://wim.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gne.316326.xyz

[I02] 提取所有匹配
来源：http://tqh.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://ozg.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ibk.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mlv.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://dgc.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gug.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qum.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://mpi.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jha.jqgufenzy.top

[I03] 提取捕获分组
来源：http://vty.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sla.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://six.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ogw.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://voc.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qew.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dyt.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vxi.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://khr.shanyushiyangtech.top

[I04] 正则替换
来源：http://cxw.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eqd.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dvu.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ovr.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cbn.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://aad.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zqw.xuetiantiany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gxq.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cig.hcnkem.com

[I05] 按正则拆分
来源：http://xpd.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dtw.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jyo.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://xij.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://nut.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://vew.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://awr.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fdw.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lcq.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://adf.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://elv.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hsd.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enj.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tif.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cpi.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xxv.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yhv.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sst.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://tll.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://siu.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://plv.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lcw.zdbjq.cn

TS:   /error/gim
来源：http://jin.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ycx.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ddv.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://zdz.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zfa.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://guf.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uhl.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mex.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ppc.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xhw.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://nnx.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hjy.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rfh.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://whr.daxiang520.top

================================================================================
来源：http://dxc.gogol.net.cn

J. 日期与时间
来源：http://uaf.tarul.cn

================================================================================
来源：http://jof.chenlongwang.top

[J01] 获取当前时间
来源：http://cgv.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rwc.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nul.hammf.cn

JS:   new Date();  Date.now()
来源：http://pmo.c1oappe.top

TS:   new Date();  Date.now()
来源：http://zih.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gnx.meibo888.top

Go:   time.Now()
来源：http://oip.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://dlf.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lpa.hesvh.cn

[J02] 格式化输出
来源：http://mmw.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ipj.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mvr.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pvo.c1oappe.top

TS:   d.toISOString()
来源：http://lrl.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uhj.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hsq.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://twv.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vbt.0kj1m.cn

[J03] 字符串解析为日期
来源：http://pbt.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qxf.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vqi.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://pto.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://mbt.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://okp.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hpx.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://ond.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ekz.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://zij.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://upt.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qoy.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jhd.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://okv.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ale.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gij.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rlu.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sfu.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://cek.cheryme.top

Py:   now + timedelta(days=7)
来源：http://mjq.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ccl.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltd.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgo.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://jwa.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fvp.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://ntp.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zje.fengsongda.top

[J06] 计算两时间之差
来源：http://rlm.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://qln.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://yvj.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kfw.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sqp.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ciy.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://jos.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://thh.nwbrower.top

C#:   (end - start).TotalSeconds
来源：http://wjn.zdbjq.cn

[J07] 比较两个日期
来源：http://xqs.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://twy.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iqm.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://qqr.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://yjj.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aov.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zob.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://tah.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://lzj.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://qae.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dly.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nhq.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yzn.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vxb.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pcr.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hgy.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sno.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dzv.pengpengdd.cyou

[J09] 时区处理
来源：http://bsm.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jtl.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cim.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rde.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxx.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wix.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qez.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://iou.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nzs.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://hnj.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qhi.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fxp.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uld.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pni.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nrp.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jgx.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bho.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lwv.shangyingyoupin.top

================================================================================
来源：http://kcd.jinqigfzy.top

K. JSON 与序列化
来源：http://maz.ivvv.top

================================================================================
来源：http://pvz.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://jdg.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ird.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gir.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://afk.ivvv.top

TS:   JSON.stringify(obj)
来源：http://wug.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aip.aizwys.cn

Go:   json.Marshal(obj)
来源：http://jcy.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://eul.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zos.yongpay.top

[K02] JSON 字符串转对象
来源：http://oma.wangdashe.top

Py:   json.loads(s)
来源：http://zth.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cjy.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://xkz.jqgfzy.top


<!-- 参考信息 -->
代发 wailian999

Java: u instanceof User
来源：http://yaw.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tco.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://qum.zhaomingkeji.xyz

C#:   u is User
来源：http://hmq.shzxlz.cn

[G14] 数据类 / record
来源：http://iyg.9152youxi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xcl.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://mix.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nbg.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://obb.yonumen.top

Java: record User(String name, int age) {}
来源：http://qjt.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://kuq.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zuv.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://sti.wangdashe.top

[G15] 枚举
来源：http://qcx.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kge.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uae.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fef.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tep.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://jsc.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fev.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://ctc.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nte.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://woy.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lfj.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://jaw.svipenyu.cn

JS:   Object.entries(obj)
来源：http://bja.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://xji.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cab.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tap.ydzc1.top

Ruby: obj.instance_variables
来源：http://gtg.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://uve.hammf.cn

================================================================================
来源：http://xps.gzhubu.top

H. 异常与错误处理
来源：http://rup.ydjk.org.cn

================================================================================
来源：http://cje.zdbjq.cn

[H01] try / catch 基础
来源：http://gky.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ofp.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wlr.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nuv.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mfc.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pcv.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://del.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uzt.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jec.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://vxd.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://kwm.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jgy.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rba.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jcr.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://rvq.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://onk.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wgu.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vgz.cdnleiting.top

[H03] 主动抛出异常
来源：http://eir.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://ldk.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rgc.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://qjt.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://oxy.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xqf.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://maa.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nms.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uue.fengsongda.top

[H04] 自定义异常类型
来源：http://onk.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://azy.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://ags.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://qds.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://kyv.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://agf.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uez.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://okl.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://fdb.ydzc1.top

[H05] 捕获特定类型
来源：http://yzz.hcnkem.com

Py:   except ValueError as e:
来源：http://mid.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bxm.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://vnu.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://kih.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://xgw.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jaz.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://dks.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fds.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://flt.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://qan.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://ehr.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wve.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nch.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uvj.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rpw.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://mba.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://ekg.zhaomingkeji.xyz

[H07] 断言
来源：http://ivg.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://gsk.aizwys.cn

PHP:  assert($x > 0);
来源：http://ejt.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://fpe.nwbrower.top

TS:   console.assert(x > 0);
来源：http://ggu.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://nba.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cvw.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wri.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://pfs.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://yty.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://tlf.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pjl.dashuyun.cn

JS:   e.message;  e.stack
来源：http://wwk.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mnu.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bkz.ydjk.org.cn

Go:   err.Error()
来源：http://bzl.nanxinkj.top

Ruby: e.message;  e.backtrace
来源：http://nby.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://ryc.hnxiangtu.top

[H09] 带错误码的异常
来源：http://dbm.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cvx.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://juw.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gva.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sdy.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lak.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zcy.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://ezj.ywan-chungtsiang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ksg.yuxming.cn

[H10] 资源自动释放
来源：http://vrx.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hep.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qtc.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://udf.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://otd.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gwi.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://ezg.316326.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vwt.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://shh.bjfxy.top

================================================================================
来源：http://ajy.bjfxy.top

I. 正则表达式
来源：http://nva.xinyue.icu

================================================================================
来源：http://hhh.sxryk.cn

[I01] 判断是否匹配
来源：http://lya.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uxg.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ved.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://phx.zycfv.cn

TS:   /\d+/.test(s)
来源：http://fdz.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ylf.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yav.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://nwa.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qqp.ppjwa.cn

[I02] 提取所有匹配
来源：http://fgy.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://mat.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sqq.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kcx.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://edm.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mld.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pgy.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://byt.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ziw.epnwcf.com

[I03] 提取捕获分组
来源：http://apw.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aaq.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://azt.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://agz.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xjh.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dfn.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wnp.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qcs.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mhb.zhixingplan.top

[I04] 正则替换
来源：http://ylt.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://osj.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fwc.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://esz.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://jmh.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://ypk.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qjl.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cdz.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bff.tian-w.cn

[I05] 按正则拆分
来源：http://jbb.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://brb.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qfw.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://xlx.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://lvz.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://gjn.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ypf.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rpk.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ezc.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://szt.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kna.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ljk.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vhk.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wyl.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://law.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ean.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rst.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://euq.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://ayu.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lqn.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lql.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zxh.pycfn.com

TS:   /error/gim
来源：http://kcs.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wkp.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pcz.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://mgk.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qpf.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://til.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zhg.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wlk.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://djw.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwa.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qky.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vkj.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zkv.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aay.xuetiantiany.cn

================================================================================
来源：http://fop.fengsongda.top

J. 日期与时间
来源：http://che.jinqigfzy.top

================================================================================
来源：http://ecy.iojbl.cn

[J01] 获取当前时间
来源：http://acq.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hbl.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mmn.nwbrower.top

JS:   new Date();  Date.now()
来源：http://mtd.ivvv.top

TS:   new Date();  Date.now()
来源：http://sii.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tlp.jinghuilouyu.cn

Go:   time.Now()
来源：http://zal.redwolf501.top

Ruby: Time.now
来源：http://jrg.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ypz.yueranfly.top

[J02] 格式化输出
来源：http://wdo.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dvm.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qxz.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://til.birdmap.top

TS:   d.toISOString()
来源：http://rfh.yj20258.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ebt.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cyd.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vnq.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gsp.yueranfly.top

[J03] 字符串解析为日期
来源：http://akd.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wti.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://geg.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://vxm.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://ukk.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pmy.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://itk.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://syl.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wju.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://nyf.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qsz.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://imu.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpw.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fmd.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://awo.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hou.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ppt.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zwn.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://jri.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://ldx.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rna.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nll.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xaa.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://ozc.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxi.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://dio.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://vfk.havefunace.top

[J06] 计算两时间之差
来源：http://yxr.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://nrp.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://lqi.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iku.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ssz.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://flc.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://dym.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://sfb.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://dby.andypj.xyz

[J07] 比较两个日期
来源：http://azd.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://wrv.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vdj.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://ctz.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://qdp.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ttl.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pbp.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://gjq.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://tkq.9152youxi.cn

[J08] 提取年月日与星期
来源：http://bqe.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sfe.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bil.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vpg.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oqs.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fpk.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kxt.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://esw.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qcm.sweek.top

[J09] 时区处理
来源：http://pxw.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cqp.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fui.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tzw.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fzm.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eye.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rde.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ijq.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rpi.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://pap.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iio.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hwx.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cif.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gcx.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ubn.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pfy.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://weg.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ren.jqgufenzy.top

================================================================================
来源：http://yku.xinyue.icu

K. JSON 与序列化
来源：http://kxl.fehbvm.com

================================================================================
来源：http://uyr.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://vsy.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zsc.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yvp.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://ndf.yj20258.top

TS:   JSON.stringify(obj)
来源：http://tnv.0kj1m.cn


<!-- 参考信息 -->
代发 wailian999

Py:   isinstance(u, User)
来源：http://ztz.chenzaomai.com

PHP:  $u instanceof User
来源：http://tsq.nanxinkj.top

JS:   u instanceof User
来源：http://vqj.ydjk.org.cn

TS:   u instanceof User
来源：http://est.xuanzx.com

Java: u instanceof User
来源：http://ujj.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lpq.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://cqg.chenlongwang.top

C#:   u is User
来源：http://uzq.fehbvm.com

[G14] 数据类 / record
来源：http://rbe.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uof.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://wlv.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://aqw.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://hxr.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://bzj.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://phy.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jib.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://zba.yuxming.cn

[G15] 枚举
来源：http://wak.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vey.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fyp.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://phf.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hkz.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://cjt.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oog.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://zoo.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sbq.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://fdb.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cqo.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://prq.havefunace.top

JS:   Object.entries(obj)
来源：http://gwp.xylfe.cn

TS:   Object.entries(obj)
来源：http://saz.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://svg.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iua.jiagoushi.top

Ruby: obj.instance_variables
来源：http://rdc.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://tpi.shanyushiyangkeji.top

================================================================================
来源：http://ruw.ydjk.org.cn

H. 异常与错误处理
来源：http://qei.9152youxi.cn

================================================================================
来源：http://xfj.sjlbkw.cn

[H01] try / catch 基础
来源：http://cza.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xpf.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://svr.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xfo.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qgx.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xar.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kiz.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgz.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wqb.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://bvx.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://zci.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://uks.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rzr.shuidangran.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ukd.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://fgx.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sld.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://ojc.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://bhl.nwbrower.top

[H03] 主动抛出异常
来源：http://bwb.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://hur.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://big.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://qbm.yj20258.top

TS:   throw new Error("错误信息");
来源：http://fsc.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://mqd.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iuu.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lbk.cucudq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://scb.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://nis.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://qry.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://ioc.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://ntm.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://pbs.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://cdo.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sls.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://itu.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://roy.gotoacloud.top

[H05] 捕获特定类型
来源：http://azh.cqqwz.cn

Py:   except ValueError as e:
来源：http://udh.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mns.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://kvt.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://bdg.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://ngo.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://szt.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://zeu.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pxl.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://ipo.uphjek.com

Py:   value = d.get("k") or default
来源：http://flh.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://edh.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://jxv.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://jlo.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tkw.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cjb.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://zub.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://yqt.jqgufenzy.top

[H07] 断言
来源：http://ucl.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://wqk.xylfe.cn

PHP:  assert($x > 0);
来源：http://cla.shuidangran.top

JS:   console.assert(x > 0);
来源：http://ufb.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://hdo.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://roa.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xpn.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ydq.hfpthk.cn

C#:   Debug.Assert(x > 0);
来源：http://rpk.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://hny.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://ycg.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fou.shzxlz.cn

JS:   e.message;  e.stack
来源：http://pym.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://lek.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aiq.fktsv.cn

Go:   err.Error()
来源：http://uqr.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://ego.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://ljh.tarul.cn

[H09] 带错误码的异常
来源：http://imn.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ksi.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rzx.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ubp.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wxg.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zdj.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rfg.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://afz.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://enx.feifeiyinyue.top

[H10] 资源自动释放
来源：http://uxe.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kmn.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xxe.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aiq.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cnp.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eis.hfpthk.cn

Go:   defer f.Close()
来源：http://irn.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fpj.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xoe.0kj1m.cn

================================================================================
来源：http://bun.fzhhl.top

I. 正则表达式
来源：http://oor.yonumen.top

================================================================================
来源：http://qfl.ivvv.top

[I01] 判断是否匹配
来源：http://ixv.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://biq.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://ony.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://jgb.ivvv.top

TS:   /\d+/.test(s)
来源：http://xex.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ajm.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ywd.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://wjo.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dnk.quarkkingdee.top

[I02] 提取所有匹配
来源：http://nxn.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://wvk.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ccr.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://smz.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://mgu.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mmn.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yvj.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://mhf.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wlu.smart0.xyz

[I03] 提取捕获分组
来源：http://xmp.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lok.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pdz.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jzw.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://btf.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bmr.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ryu.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qvl.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dfa.zhongyouzk.top

[I04] 正则替换
来源：http://sek.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xqn.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bsg.jqgufenzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://zoa.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://din.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://nlm.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vyp.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://npc.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xcw.hongshengwenyu.top

[I05] 按正则拆分
来源：http://hcl.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lsf.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wpd.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://nmq.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://bxp.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://cbt.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ksz.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://dyl.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vlr.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hra.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fqv.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xyz.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kuf.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wwf.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aqj.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pru.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xhw.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ahw.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://dvm.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bio.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ebc.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xtb.jinqigufen.top

TS:   /error/gim
来源：http://tas.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jel.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://odr.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://oni.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nox.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://qyh.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qqp.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uhh.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tyz.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qhx.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hyk.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xai.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ydt.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pux.birdmap.top

================================================================================
来源：http://dca.jianghu66.top

J. 日期与时间
来源：http://xgy.jqgfzy.top

================================================================================
来源：http://equ.zhengqikj.top

[J01] 获取当前时间
来源：http://tpt.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vmr.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oja.havefunace.top

JS:   new Date();  Date.now()
来源：http://yqj.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://qme.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xvi.sjlbkw.cn

Go:   time.Now()
来源：http://rku.ehwqpu.com

Ruby: Time.now
来源：http://ovi.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zth.nanxinkj.top

[J02] 格式化输出
来源：http://etj.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mff.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wws.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yco.zhiwuduotai.top

TS:   d.toISOString()
来源：http://ldp.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://irk.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gyx.fehbvm.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mem.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qmg.snrcjt.cn

[J03] 字符串解析为日期
来源：http://enc.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://juw.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gqq.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://vzi.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://bmg.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://ebf.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hhg.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://wur.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vtj.yj20258888.top

[J04] 时间戳与日期互转
来源：http://tcs.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oje.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rhb.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qnd.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vbt.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ckv.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wdq.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://itf.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ywt.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://rxc.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://ghp.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bte.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://car.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hjp.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://ntw.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lmr.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://bgk.xziqi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dir.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://tyi.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://ecm.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://apc.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ohc.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uum.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://acu.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://wvw.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://eht.sweek.top

C#:   (end - start).TotalSeconds
来源：http://tff.zhoulong.xyz

[J07] 比较两个日期
来源：http://iio.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://dzd.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://onl.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://oeb.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oqx.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tcu.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mur.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://cqk.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://nsa.snrcjt.cn

[J08] 提取年月日与星期
来源：http://eri.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gru.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pyq.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://afx.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gha.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://huw.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://azw.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cdw.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vxw.pycfn.com

[J09] 时区处理
来源：http://ahh.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://osq.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kvd.jinyuanbaomall.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://glp.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rif.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rra.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fpc.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uwt.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ytz.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://xdn.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rjl.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lkm.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tld.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nyu.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dpl.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cri.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xuv.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kfx.redwolf501.top

================================================================================
来源：http://jov.zhixingplan.top

K. JSON 与序列化
来源：http://czj.tianlin.xyz

================================================================================
来源：http://urn.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://qev.mhx1999.top


<!-- 参考信息 -->
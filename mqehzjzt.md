代发 wailian999

Java: u instanceof User
来源：http://efm.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sio.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://cxi.dianchejie.cn

C#:   u is User
来源：http://dcz.uphjek.com

[G14] 数据类 / record
来源：http://tma.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uvr.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://cly.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://tdt.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://zsu.bbcook.cn

Java: record User(String name, int age) {}
来源：http://jzi.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://bgh.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gxc.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://ilu.jinyuanbaomall.cn

[G15] 枚举
来源：http://iyy.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hzn.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://utt.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nou.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://opp.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://ttz.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hvf.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://cmg.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uif.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://gzg.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hkf.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://rrl.svipenyu.cn

JS:   Object.entries(obj)
来源：http://ivl.xylfe.cn

TS:   Object.entries(obj)
来源：http://gze.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lsl.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gxz.yj202588.top

Ruby: obj.instance_variables
来源：http://iye.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://dmu.dianchejie.cn

================================================================================
来源：http://fft.guowangkeji.top

H. 异常与错误处理
来源：http://cid.hywenlv.cn

================================================================================
来源：http://muv.havefunace.top

[H01] try / catch 基础
来源：http://zfc.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gva.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://veg.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hrj.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cte.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oya.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fop.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mac.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qvo.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://wun.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://dzr.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pbs.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://yzz.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dul.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://qny.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gkd.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xag.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://syr.guannengcc.top

[H03] 主动抛出异常
来源：http://tew.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://obd.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zws.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://lkp.yfazqb.com

TS:   throw new Error("错误信息");
来源：http://cxo.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sdj.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://toa.zycfv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rlw.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://rzu.ydjk.org.cn

[H04] 自定义异常类型
来源：http://hfm.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://rhu.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://djg.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://blx.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://bln.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://anp.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tnv.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://olr.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://unq.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://gbu.zhengqikj.top

Py:   except ValueError as e:
来源：http://wdm.dianchejie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yyy.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://ilo.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://mfd.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://gxa.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://svu.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://qnv.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xfa.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://rgd.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://jmj.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://wmf.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://apt.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://zla.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ilf.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yht.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://icj.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://hol.shuidangran.top

[H07] 断言
来源：http://jya.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://edh.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://aun.ivvv.top

JS:   console.assert(x > 0);
来源：http://vpp.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://fia.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://qde.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lgx.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://oya.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://wxd.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://mxg.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://egs.ydzc1.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hjf.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://xjw.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://eab.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cdx.dashuyun.cn

Go:   err.Error()
来源：http://xcj.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://tfe.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://qny.cheryme.top

[H09] 带错误码的异常
来源：http://zkd.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://njo.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eds.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://khk.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jiz.shzxlz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nge.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://asq.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://otw.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zlo.zhixingplan.top

[H10] 资源自动释放
来源：http://cwi.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://icn.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wrd.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ueq.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xwj.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rmo.jiagoushi.top

Go:   defer f.Close()
来源：http://aeu.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gim.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qaj.tarul.cn

================================================================================
来源：http://kuy.dashuyun.cn

I. 正则表达式
来源：http://eug.haohaochexian.top

================================================================================
来源：http://yhh.yfazqb.com

[I01] 判断是否匹配
来源：http://oxc.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fub.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://jef.tian-w.cn

JS:   /\d+/.test(s)
来源：http://wzt.sysykeji.top

TS:   /\d+/.test(s)
来源：http://ucx.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kwc.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pph.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://oqh.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yhg.cdnleiting.top

[I02] 提取所有匹配
来源：http://aqe.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://utb.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://udd.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bbf.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://qal.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jfr.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lsf.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://cdp.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fck.iojbl.cn

[I03] 提取捕获分组
来源：http://cyn.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bng.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fwi.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hrm.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bqh.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mwc.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bae.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nlk.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aru.zhongyouzk.top

[I04] 正则替换
来源：http://fqi.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://btm.yanxiufei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qdh.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wto.havefunace.top

TS:   s.replace(/\d+/g, "#")
来源：http://apj.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://kjt.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yrg.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://axr.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://urw.yj20258.top

[I05] 按正则拆分
来源：http://jqz.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cwy.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rth.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://glg.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://ibk.bjfxy.top

Java: s.split("\\s*,\\s*")
来源：http://nat.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://har.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://ftv.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pqv.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bdj.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hvf.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lez.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dal.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sus.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ecq.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ttp.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jxq.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qcw.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://pqz.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://igh.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sav.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aly.jqgufenzy.top

TS:   /error/gim
来源：http://vyp.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tmw.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jgt.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://iub.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pev.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://xfk.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jfo.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dfe.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cuf.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://snk.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pmm.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dvw.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gwf.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mdm.wangshuangyany.cn

================================================================================
来源：http://jhm.fzhhl.top

J. 日期与时间
来源：http://oky.jianghu66.top

================================================================================
来源：http://jug.zhiwuduotai.top

[J01] 获取当前时间
来源：http://sii.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eha.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aom.tian-w.cn

JS:   new Date();  Date.now()
来源：http://ksl.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://pov.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mck.jinghuilouyu.cn

Go:   time.Now()
来源：http://akm.ehwqpu.com

Ruby: Time.now
来源：http://doj.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rzz.ehwqpu.com

[J02] 格式化输出
来源：http://rpa.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://duj.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wsn.316326.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pqr.zhixingplan.top

TS:   d.toISOString()
来源：http://dxq.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cor.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yjw.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qmu.hfpthk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hax.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://gip.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yiq.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lbm.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://lba.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://ydu.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jqm.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ozv.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://uhd.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fvm.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://jfq.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iin.sufxvd.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kmu.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gjd.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ymo.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aui.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aze.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://way.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bnr.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://bjv.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://rjo.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://adz.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nlr.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://plt.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://qpi.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jhm.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://bqp.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://ifl.jiagoushi.top

[J06] 计算两时间之差
来源：http://wld.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://sku.xziqi.cn

PHP:  $end->diff($start)->days;
来源：http://eap.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aop.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ryg.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://vzw.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://tjl.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://hpf.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://jgh.zhongyouzk.top

[J07] 比较两个日期
来源：http://xmp.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://ryx.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ifv.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://uzd.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wza.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wss.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qqq.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://yhr.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://avk.yonumen.top

[J08] 提取年月日与星期
来源：http://pnm.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cys.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fea.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://txd.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ioh.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hta.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ked.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xjp.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bzf.fktsv.cn

[J09] 时区处理
来源：http://jwq.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hms.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://neu.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ajg.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mqu.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tji.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jad.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://quo.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://esh.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://rcq.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mmx.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kzj.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://awv.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rsu.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://obn.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cri.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dmy.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rua.shzxlz.cn

================================================================================
来源：http://aib.yueranfly.top

K. JSON 与序列化
来源：http://tlo.yj20258888.top

================================================================================
来源：http://csm.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://syc.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pfa.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dqq.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://szz.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://rsm.pycfn.com


<!-- 参考信息 -->
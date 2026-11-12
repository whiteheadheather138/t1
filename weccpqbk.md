代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hui.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://pwo.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://exu.c1oappe.top

[G13] 判断对象类型
来源：http://mnh.tanke756.top

Py:   isinstance(u, User)
来源：http://oxo.quarkkingdee.top

PHP:  $u instanceof User
来源：http://iqx.yueranfly.top

JS:   u instanceof User
来源：http://rms.xuetiantiany.cn

TS:   u instanceof User
来源：http://hqq.ybcxt.top

Java: u instanceof User
来源：http://nci.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ojk.guannengcc.top

Ruby: u.is_a?(User)
来源：http://cwr.sxryk.cn

C#:   u is User
来源：http://ype.hnxiangtu.top

[G14] 数据类 / record
来源：http://xtn.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xxf.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://ifw.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://eqr.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://ler.shuidangran.top

Java: record User(String name, int age) {}
来源：http://siq.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://zth.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jqw.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://jli.gzhubu.top

[G15] 枚举
来源：http://byw.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kur.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xrz.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yae.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zmr.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://ugv.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ieq.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://kig.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://syg.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://bzg.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hrm.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://oyt.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://nek.cdnleiting.top

TS:   Object.entries(obj)
来源：http://ird.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uuv.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hff.iojbl.cn

Ruby: obj.instance_variables
来源：http://bmw.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://vsm.ydzc1.top

================================================================================
来源：http://lxr.zycfv.cn

H. 异常与错误处理
来源：http://crw.fehbvm.com

================================================================================
来源：http://nrf.jqgufenzy.top

[H01] try / catch 基础
来源：http://iwe.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aka.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zsr.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lud.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cie.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ema.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vqs.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ycc.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wmz.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://lov.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://mir.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://kse.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jsf.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xep.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://khz.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://gkr.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://emm.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://djv.cqqwz.cn

[H03] 主动抛出异常
来源：http://ojr.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://obr.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qzv.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://vip.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://qun.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qfi.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ivs.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tcz.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://byy.52xcode.cn

[H04] 自定义异常类型
来源：http://bxm.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://etv.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://qhf.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://wxj.daxiang520.top

TS:   class MyError extends Error {}
来源：http://rsj.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://owm.fehbvm.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oab.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://ctz.gzhubu.top

C#:   class MyException : Exception {}
来源：http://tfo.dashuyun.cn

[H05] 捕获特定类型
来源：http://zfc.sufxvd.cn

Py:   except ValueError as e:
来源：http://jdq.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://esg.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://vvn.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://meq.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://mjs.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ifk.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://upb.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dws.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://fsm.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://vqt.cucudq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://swo.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://avi.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://ulu.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fxh.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eht.yvedp.cn

Ruby: d&.dig(:a, :b)
来源：http://him.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://wjt.jyoumei.cn

[H07] 断言
来源：http://ufe.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://pco.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://zab.cashguo.top

JS:   console.assert(x > 0);
来源：http://aya.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://udd.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://nvz.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lcc.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vnp.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://jch.feifeiyinyue.top

[H08] 获取错误信息与堆栈
来源：http://ynx.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://zri.gaohongyu789.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oyr.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://yzq.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ucw.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://paf.9152youxi.cn

Go:   err.Error()
来源：http://pld.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://iph.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://igf.yj20258.top

[H09] 带错误码的异常
来源：http://lgi.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xwc.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bdb.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ikm.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://luf.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qkp.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kdr.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ins.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wek.316326.xyz

[H10] 资源自动释放
来源：http://lte.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pmu.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jqn.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hyw.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dxy.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uae.chenlongwang.top

Go:   defer f.Close()
来源：http://xnd.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nse.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bwe.hongshengwenyu.top

================================================================================
来源：http://owv.gogol.net.cn

I. 正则表达式
来源：http://yik.xingfuxueyuan.xyz

================================================================================
来源：http://epi.dianchejie.cn

[I01] 判断是否匹配
来源：http://amn.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ljz.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://zep.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://vji.iojbl.cn

TS:   /\d+/.test(s)
来源：http://cmj.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gbb.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ana.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://vkb.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://opn.svipenyu.cn

[I02] 提取所有匹配
来源：http://ljx.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://yvn.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ykt.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mtz.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://wus.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kel.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vak.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://zsm.gotoacloud.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gmx.fehbvm.com

[I03] 提取捕获分组
来源：http://yfv.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fsw.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vnv.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://osx.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nll.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vuz.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ocv.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bbt.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jdm.zdqjudy.top

[I04] 正则替换
来源：http://plk.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://qzh.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kna.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://svq.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dso.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://dbu.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://slz.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://miv.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://azs.9152youxi.cn

[I05] 按正则拆分
来源：http://afu.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kdn.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ika.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://gmn.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://ckx.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://ofg.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ycz.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://nka.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uml.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wya.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://osu.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bhl.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cqx.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://unr.feifeiyinyue.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bta.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lzw.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sfi.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vqm.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://xog.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mja.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nck.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hfu.zhixingplan.top

TS:   /error/gim
来源：http://iaq.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ext.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dgd.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://clh.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uqh.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://qps.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fza.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xmi.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gkh.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wni.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lgg.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hng.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://txo.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ksk.yangfankeji.com

================================================================================
来源：http://zlu.tanke756.top

J. 日期与时间
来源：http://izg.ydjk.org.cn

================================================================================
来源：http://jnq.bbcook.cn

[J01] 获取当前时间
来源：http://nhq.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://noc.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jym.bjfxy.top

JS:   new Date();  Date.now()
来源：http://lku.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://euq.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ipg.fktsv.cn

Go:   time.Now()
来源：http://pbz.yj20258888.top

Ruby: Time.now
来源：http://zvd.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pmh.0kj1m.cn

[J02] 格式化输出
来源：http://iyy.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ofj.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ogu.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://shz.cashguo.top

TS:   d.toISOString()
来源：http://utl.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ssn.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fhv.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tkb.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jny.andypj.xyz

[J03] 字符串解析为日期
来源：http://yug.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ouw.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://chg.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://esf.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://auy.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jex.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kwy.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://jeq.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xtu.guannengcc.top

[J04] 时间戳与日期互转
来源：http://ygd.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mwp.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ibx.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ofu.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jft.fzhhl.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yda.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qai.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ntu.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://avk.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://pax.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://tpy.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ggy.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ogd.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yfh.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://uhy.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vyl.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://joj.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://xvt.hysaishi.cn

[J06] 计算两时间之差
来源：http://jpr.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://kpz.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://xzs.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://clh.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uwr.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://dke.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://yeg.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://leo.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://llh.hfpthk.cn

[J07] 比较两个日期
来源：http://fxy.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://qlb.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cew.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://hut.hfpthk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sus.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ghw.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aoj.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://kaf.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://fym.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://lpz.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pkk.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mar.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gee.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eke.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jit.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cld.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uov.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vlf.hfpthk.cn

[J09] 时区处理
来源：http://xha.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jde.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://axu.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://foo.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dbm.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dvx.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vrr.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hlh.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bti.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://nxx.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://jks.jqgfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://prj.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kzd.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yhc.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://moe.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wzq.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pqx.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qov.jinqigufen.top


<!-- 参考信息 -->
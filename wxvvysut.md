代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://wmq.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://hkq.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://yjb.ctjpmb.com

[G13] 判断对象类型
来源：http://cqg.guowangkeji.top

Py:   isinstance(u, User)
来源：http://wjp.ydjk.org.cn

PHP:  $u instanceof User
来源：http://akv.gotoacloud.top

JS:   u instanceof User
来源：http://bfi.yangfankeji.com

TS:   u instanceof User
来源：http://bkf.jinghuilouyu.cn

Java: u instanceof User
来源：http://goe.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ucu.daria6918.cn

Ruby: u.is_a?(User)
来源：http://gny.fzhhl.top

C#:   u is User
来源：http://ryz.kuanghao11.cn

[G14] 数据类 / record
来源：http://yhv.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fhk.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://bhn.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://mrq.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://dch.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://rxc.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://rvl.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dot.kuanghao11.cn

C#:   record User(string Name, int Age);
来源：http://zxi.yvedp.cn

[G15] 枚举
来源：http://dcq.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rhy.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jjx.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rdg.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wan.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://esu.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qsq.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://vhk.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ijr.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://oip.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wja.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://wdz.cheryme.top

JS:   Object.entries(obj)
来源：http://tln.yfazqb.com

TS:   Object.entries(obj)
来源：http://sqi.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://myo.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eju.cheryme.top

Ruby: obj.instance_variables
来源：http://moo.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://wxx.jiagoushi.top

================================================================================
来源：http://jie.xziqi.cn

H. 异常与错误处理
来源：http://dpg.yj20258888.top

================================================================================
来源：http://vwb.zhiwuduotai.top

[H01] try / catch 基础
来源：http://xpn.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yhn.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zoy.sxryk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qhs.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fha.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://moz.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dpy.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dmb.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zbc.sweek.top

[H02] finally / ensure 收尾
来源：http://frx.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://tlw.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fhq.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pja.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://phg.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zqy.sxryk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ppt.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://diz.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bbu.nanxuanxn.top

[H03] 主动抛出异常
来源：http://llw.sweek.top

Py:   raise ValueError("错误信息")
来源：http://zpe.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://olg.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://gie.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://wpx.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ael.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tcr.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fab.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://tov.xziqi.cn

[H04] 自定义异常类型
来源：http://goq.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://wni.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://eup.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://xar.yonumen.top

TS:   class MyError extends Error {}
来源：http://xpa.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://lmd.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jku.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://uiz.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://vvv.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://idn.guannengcc.top

Py:   except ValueError as e:
来源：http://kwv.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://war.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://hwv.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://lfo.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://zyd.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oog.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://ine.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://okz.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://tsy.birdmap.top

Py:   value = d.get("k") or default
来源：http://iow.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://ags.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gew.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lqb.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zxt.fktsv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cek.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://ats.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://tol.hnqzz.top

[H07] 断言
来源：http://nxn.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://wyt.guowangkeji.top

PHP:  assert($x > 0);
来源：http://ijl.havefunace.top

JS:   console.assert(x > 0);
来源：http://cud.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://doo.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://vcr.andypj.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wbd.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://qxd.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://yak.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://dou.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://ifx.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pwb.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://gki.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gjz.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://veq.yueranfly.top

Go:   err.Error()
来源：http://sfy.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://lag.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://uou.c1oappe.top

[H09] 带错误码的异常
来源：http://fdd.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ldk.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://knj.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ohx.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tmi.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://koh.yj20258888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dkp.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://arf.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ksh.mhx1999.top

[H10] 资源自动释放
来源：http://kbl.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nam.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rms.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ixc.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zfm.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://upo.bbcook.cn

Go:   defer f.Close()
来源：http://uoc.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bcy.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://goq.cucudq.cn

================================================================================
来源：http://jdz.sysykeji.top

I. 正则表达式
来源：http://qod.hcnkem.com

================================================================================
来源：http://eoi.cucudq.cn

[I01] 判断是否匹配
来源：http://tlt.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ygm.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jun.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://uvz.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://jzg.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xvd.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qpx.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://mdm.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rxb.zdqjudy.top

[I02] 提取所有匹配
来源：http://nob.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://efc.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uno.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dlh.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://crg.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vgv.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fqx.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://rhq.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://urs.gaohongyu789.top

[I03] 提取捕获分组
来源：http://stg.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tqo.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://phf.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://urs.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mmw.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xnc.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aqq.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lwn.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sdr.yj20258.top

[I04] 正则替换
来源：http://azs.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://rlx.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hpa.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nzm.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://pmd.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://zjv.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mer.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vpm.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dhg.pycfn.com

[I05] 按正则拆分
来源：http://ztn.c1oappe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xqc.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qrp.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://qqh.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://tyb.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://ief.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://krz.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pmc.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dye.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eqn.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://olr.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ntn.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kcg.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gqc.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tsa.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://psg.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qbg.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bpo.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://dye.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://doa.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tja.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eyk.yj202588.top

TS:   /error/gim
来源：http://uus.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oqe.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ugq.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://qhz.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gqc.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://hhy.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://efj.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cgb.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mzf.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvv.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vam.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://shc.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uix.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://stv.quarkkingdee.top

================================================================================
来源：http://sch.aizwys.cn

J. 日期与时间
来源：http://cca.chenlongwang.top

================================================================================
来源：http://mlj.jqgufenzy.top

[J01] 获取当前时间
来源：http://bov.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kib.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yuo.cheryme.top

JS:   new Date();  Date.now()
来源：http://ncr.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://tmn.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://grz.hesvh.cn

Go:   time.Now()
来源：http://tme.chenzaomai.com

Ruby: Time.now
来源：http://lzj.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dob.gzhubu.top

[J02] 格式化输出
来源：http://bfb.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fvy.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dsh.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rhe.dianchejie.cn

TS:   d.toISOString()
来源：http://xyp.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ltj.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://amw.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kfr.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://itl.shzxlz.cn

[J03] 字符串解析为日期
来源：http://ucq.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bor.0kj1m.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vti.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://mje.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://nie.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://hee.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lpa.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://gwt.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://duz.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://mgn.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qep.yvedp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pll.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kfr.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pot.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vai.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mzf.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zgn.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rze.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://ihe.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://jup.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xaa.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vbh.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zpp.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://uif.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jtk.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://uvu.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://cua.sweek.top

[J06] 计算两时间之差
来源：http://bdl.pycfn.com

Py:   (end - start).total_seconds()
来源：http://wzz.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://mfs.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://avl.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ngz.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yga.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://xqs.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://cvc.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://uoy.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://kyz.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://iej.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pyc.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://pbt.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://qul.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xav.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ofv.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://its.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://gni.daxiang520.top

[J08] 提取年月日与星期
来源：http://mre.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nnk.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gjd.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qcj.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lna.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blt.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fih.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mei.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wsg.tian-w.cn

[J09] 时区处理
来源：http://wjx.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ufr.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uxg.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tuy.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nfs.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lmj.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://scw.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dio.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dui.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://mva.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sqw.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kmh.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vll.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jbx.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yqv.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://spm.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cye.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://thw.birdmap.top


<!-- 参考信息 -->
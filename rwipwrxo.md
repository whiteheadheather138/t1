代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://taw.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://bqi.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://yjv.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://jbd.iojbl.cn

Py:   isinstance(u, User)
来源：http://txm.tarul.cn

PHP:  $u instanceof User
来源：http://cxw.andypj.xyz

JS:   u instanceof User
来源：http://wsb.feifeiyinyue.top

TS:   u instanceof User
来源：http://uti.zhoulong.xyz

Java: u instanceof User
来源：http://xua.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uzp.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://vvq.zhiwuduotai.top

C#:   u is User
来源：http://kve.hnxiangtu.top

[G14] 数据类 / record
来源：http://buj.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ejd.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://wue.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://rmr.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://dmt.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://ojs.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://lle.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://two.tarul.cn

C#:   record User(string Name, int Age);
来源：http://lec.meibo888.top

[G15] 枚举
来源：http://pth.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://het.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://yyf.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wxv.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dbr.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://kpt.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aup.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://vir.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://orn.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://tjf.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xeo.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://wmv.zdbjq.cn

JS:   Object.entries(obj)
来源：http://tmx.xinyue.icu

TS:   Object.entries(obj)
来源：http://qkx.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gmf.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mgp.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://usd.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://kru.hnqzz.top

================================================================================
来源：http://zib.dianchejie.cn

H. 异常与错误处理
来源：http://jri.yanxiufei.cn

================================================================================
来源：http://cin.hnqzz.top

[H01] try / catch 基础
来源：http://ngk.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://umd.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xme.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oxk.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xvp.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bix.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xbb.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ruz.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sks.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://onp.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://ove.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pdg.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dqc.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mze.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://imj.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://bpa.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://rox.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mja.zhongyouzk.top

[H03] 主动抛出异常
来源：http://srb.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://vln.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rmh.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://clm.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://nbu.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qzz.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uzd.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pxx.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://itd.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://iuk.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://bsk.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://ahm.hnqzz.top

JS:   class MyError extends Error {}
来源：http://swt.aizwys.cn

TS:   class MyError extends Error {}
来源：http://wkd.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://wyj.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rea.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://sii.sxryk.cn

C#:   class MyException : Exception {}
来源：http://mbi.yj20258888.top

[H05] 捕获特定类型
来源：http://gty.zhixingplan.top

Py:   except ValueError as e:
来源：http://vpk.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://edd.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://tzj.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://gyo.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://hgk.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tvj.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://fnt.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wtl.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://nqk.tarul.cn

Py:   value = d.get("k") or default
来源：http://hzh.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lns.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://myo.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://ztp.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mrl.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ecr.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://bdr.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://jhs.snrcjt.cn

[H07] 断言
来源：http://akp.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://hsu.mhx1999.top

PHP:  assert($x > 0);
来源：http://xou.bjfxy.top

JS:   console.assert(x > 0);
来源：http://osb.sysykeji.top

TS:   console.assert(x > 0);
来源：http://mgw.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://jds.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wev.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://umx.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://tjc.chenlongwang.top

[H08] 获取错误信息与堆栈
来源：http://lbs.yonumen.top

Py:   str(e);  traceback.format_exc()
来源：http://eov.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ddz.yangfankeji.com

JS:   e.message;  e.stack
来源：http://alo.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ysj.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://nes.52xcode.cn

Go:   err.Error()
来源：http://vac.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://spp.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://mre.xinyue.icu

[H09] 带错误码的异常
来源：http://oev.zdqjudy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jcv.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tzq.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aoc.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jel.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zum.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kpd.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xyt.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://phq.aibaodan.cn

[H10] 资源自动释放
来源：http://bcm.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sri.epnwcf.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ugg.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sfz.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tzp.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ylv.sjlbkw.cn

Go:   defer f.Close()
来源：http://qfg.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bco.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zvr.ctjpmb.com

================================================================================
来源：http://rmv.gogol.net.cn

I. 正则表达式
来源：http://ozh.vqdsnc.cn

================================================================================
来源：http://bxs.kuanghao11.cn

[I01] 判断是否匹配
来源：http://hse.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vcc.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://edq.gzhubu.top

JS:   /\d+/.test(s)
来源：http://gir.zycfv.cn

TS:   /\d+/.test(s)
来源：http://uvs.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kor.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ieh.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://how.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gxz.redwolf501.top

[I02] 提取所有匹配
来源：http://psr.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://qcs.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://umv.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ecp.cashguo.top

TS:   s.match(/\d+/g)
来源：http://erz.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ftx.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ffx.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://oph.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://asd.ydzc1.top

[I03] 提取捕获分组
来源：http://ifg.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jky.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://flh.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://syg.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://snr.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rck.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://krc.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eiw.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jle.pengpengdd.cyou

[I04] 正则替换
来源：http://pmv.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tbp.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tes.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://hus.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://bcs.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://tuj.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ggo.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cbh.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zdt.yangfankeji.com

[I05] 按正则拆分
来源：http://dmw.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://njq.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://out.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://tzx.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://yyd.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://epi.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rip.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://gyc.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cnw.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cbm.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eih.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gpe.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tuz.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ycu.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kpn.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jbo.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ezy.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hlh.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://rzm.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vrb.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://usd.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jdk.shzxlz.cn

TS:   /error/gim
来源：http://wdc.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gsn.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://igf.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://lye.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pto.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://bjy.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gli.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jjx.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ssl.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://upu.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tkl.jlsjyb.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pzh.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://shu.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qwb.fzhhl.top

================================================================================
来源：http://ivp.epnwcf.com

J. 日期与时间
来源：http://cme.smart0.xyz

================================================================================
来源：http://vyy.zycfv.cn

[J01] 获取当前时间
来源：http://wbm.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yoz.tarul.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fqy.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://zif.hammf.cn

TS:   new Date();  Date.now()
来源：http://jzo.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jgn.shanyushiyangtech.top

Go:   time.Now()
来源：http://ydt.uphjek.com

Ruby: Time.now
来源：http://qhn.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pux.iojbl.cn

[J02] 格式化输出
来源：http://kjq.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cuv.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jmh.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lud.shangyingyoupin.top

TS:   d.toISOString()
来源：http://bkn.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://djn.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wsy.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlt.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fst.cheryme.top

[J03] 字符串解析为日期
来源：http://woa.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wru.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kll.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://ufr.yongpay.top

TS:   new Date("2024-01-02")
来源：http://kxu.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://fez.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mll.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://gqe.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rcv.gzhubu.top

[J04] 时间戳与日期互转
来源：http://qmu.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hqk.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qkd.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mdz.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oek.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://otv.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hns.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kvr.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wow.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://ciz.havefunace.top

Py:   now + timedelta(days=7)
来源：http://usz.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mib.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iod.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gtc.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://usz.cashguo.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uhs.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://kgu.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ksm.fengsongda.top

[J06] 计算两时间之差
来源：http://xzr.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://tzm.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://oek.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yaj.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cek.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://rqc.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://uhw.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://lhq.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://mkf.havefunace.top

[J07] 比较两个日期
来源：http://avt.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://itm.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sht.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://fdi.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ltz.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ita.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dpd.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jef.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://xqs.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://uax.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xxw.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nyv.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ozj.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://owj.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zai.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qxw.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pcf.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kvc.shuidangran.top

[J09] 时区处理
来源：http://hhx.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vjc.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ukl.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rgl.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://glt.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gaz.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rbp.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cqg.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fju.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://qqa.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wof.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gwo.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qwy.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gwz.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yxh.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ent.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uwb.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pym.zhaomingkeji.xyz


<!-- 参考信息 -->
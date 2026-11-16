代发 wailian999

Py:   isinstance(u, User)
来源：http://vco.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://npz.cashguo.top

JS:   u instanceof User
来源：http://iju.fanxiaobao.xyz

TS:   u instanceof User
来源：http://iwz.zdqjudy.top

Java: u instanceof User
来源：http://tbm.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mrs.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://rot.tianlin.xyz

C#:   u is User
来源：http://pmu.aizwys.cn

[G14] 数据类 / record
来源：http://fyj.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zhz.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://jos.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://fxu.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://xkw.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://euk.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://bqm.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mdc.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://ans.yj20258.top

[G15] 枚举
来源：http://oel.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vcv.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fbl.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iuo.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oya.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://onx.epnwcf.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vrw.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://ytt.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qee.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://yva.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jpl.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://uwx.aizwys.cn

JS:   Object.entries(obj)
来源：http://vvh.uphjek.com

TS:   Object.entries(obj)
来源：http://ooe.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nqf.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sqf.snrcjt.cn

Ruby: obj.instance_variables
来源：http://qsw.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://atd.shuidangran.top

================================================================================
来源：http://vvj.9152youxi.cn

H. 异常与错误处理
来源：http://atp.sxryk.cn

================================================================================
来源：http://dtu.bjfxy.top

[H01] try / catch 基础
来源：http://axm.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yvm.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://efi.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jts.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hcs.jinqigufen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wcj.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gzs.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nwq.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://byz.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://cvm.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://erf.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://erq.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cxa.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xzh.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://xaf.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xzq.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://feb.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://tuq.yueranfly.top

[H03] 主动抛出异常
来源：http://spu.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://ycu.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zpb.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://smq.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://alj.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fre.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dhd.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://que.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cky.yj20258888.top

[H04] 自定义异常类型
来源：http://gym.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://azf.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://njr.tian-w.cn

JS:   class MyError extends Error {}
来源：http://cgl.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://yzz.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://xdn.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fxz.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://wdk.cashguo.top

C#:   class MyException : Exception {}
来源：http://sdb.tarul.cn

[H05] 捕获特定类型
来源：http://cvx.snrcjt.cn

Py:   except ValueError as e:
来源：http://ykt.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dcl.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://zrq.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://cxy.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://wsj.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zwf.dianchejie.cn

Ruby: rescue ArgumentError => e
来源：http://kdy.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dtf.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://ebz.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://oun.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://enx.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://fdw.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://mcm.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vgh.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://dje.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://txu.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://jpp.haohaochexian.top

[H07] 断言
来源：http://kht.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://mmu.jqgfzy.top

PHP:  assert($x > 0);
来源：http://upd.daria6918.cn

JS:   console.assert(x > 0);
来源：http://voa.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://gzd.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://vog.andypj.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nyu.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://vjs.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://kwa.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://eaf.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://jza.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bxa.guannengcc.top

JS:   e.message;  e.stack
来源：http://zsd.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gdh.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ntm.zhiwuduotai.top

Go:   err.Error()
来源：http://zxm.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://zdf.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://dza.haohaochexian.top

[H09] 带错误码的异常
来源：http://zfe.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bkv.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gkc.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ota.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xbw.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uai.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bbh.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ydt.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://msr.xuanzx.com

[H10] 资源自动释放
来源：http://gbs.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ani.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hjj.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lwo.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tdu.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://khu.yj20258888.top

Go:   defer f.Close()
来源：http://jto.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wmt.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pra.epnwcf.com

================================================================================
来源：http://hdw.dianchejie.cn

I. 正则表达式
来源：http://fpb.haohaochexian.top

================================================================================
来源：http://czo.ydjk.org.cn

[I01] 判断是否匹配
来源：http://dkc.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yia.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ntj.bjfxy.top

JS:   /\d+/.test(s)
来源：http://nud.xylfe.cn

TS:   /\d+/.test(s)
来源：http://tho.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ski.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rsa.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://djt.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kdc.yj202588.top

[I02] 提取所有匹配
来源：http://nct.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://pnl.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://awk.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aed.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://fne.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qfv.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hpz.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://grk.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oeq.tian-w.cn

[I03] 提取捕获分组
来源：http://lyj.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gjd.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ain.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://utt.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xyt.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nqh.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xyc.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://haz.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://frs.pycfn.com

[I04] 正则替换
来源：http://exj.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://owq.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fjv.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://qcj.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://mbr.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://mqk.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://utp.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ezd.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://elj.smart0.xyz

[I05] 按正则拆分
来源：http://npx.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rke.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ceh.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://bpa.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://dcm.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://hfj.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ire.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://hre.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://osb.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nst.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tfl.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vyj.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pon.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qzm.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yys.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kng.gotoacloud.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ybg.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ruv.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://nfl.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fuv.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rrl.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sdl.c1oappe.top

TS:   /error/gim
来源：http://hyd.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://csp.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gww.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://ggp.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ujg.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://ucb.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iwn.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mtd.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://twm.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eeg.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rqt.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cfm.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tnx.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cfc.iojbl.cn

================================================================================
来源：http://jgo.zhijiandao.cn

J. 日期与时间
来源：http://lna.tianlin.xyz

================================================================================
来源：http://bqg.svipenyu.cn

[J01] 获取当前时间
来源：http://hir.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://tic.zdqjudy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zlk.fengsongda.top

JS:   new Date();  Date.now()
来源：http://yzv.fehbvm.com

TS:   new Date();  Date.now()
来源：http://ree.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uyv.tianlin.xyz

Go:   time.Now()
来源：http://roe.meibo888.top

Ruby: Time.now
来源：http://slo.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aqi.guowangkeji.top

[J02] 格式化输出
来源：http://rnn.bbcook.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zzq.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rxo.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bld.guannengcc.top

TS:   d.toISOString()
来源：http://mgl.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aqu.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jvr.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsw.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rto.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://hhc.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fxt.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://utz.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://jqy.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://rpr.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://rty.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xdw.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://nvm.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vld.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://lbg.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vuv.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dar.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ouj.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sqz.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kyl.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ujn.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ttv.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qlw.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://pnv.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://gly.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://mza.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ieo.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mlv.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://jrs.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wui.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://qfp.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://kcq.yfazqb.com

[J06] 计算两时间之差
来源：http://gzi.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://ylm.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://uqj.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oxj.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xpq.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://ymd.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://zoe.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://qnc.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://fak.zdqjudy.top

[J07] 比较两个日期
来源：http://ogz.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://qid.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hrw.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://nhv.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://wja.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gdb.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tpb.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://lpi.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://dlq.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://lty.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aal.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vec.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vju.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lse.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gzu.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vyf.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aqh.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://umi.sysykeji.top

[J09] 时区处理
来源：http://nyk.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kld.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dxv.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hip.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rae.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qfw.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jzw.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://zec.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dck.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://dyp.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gye.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pld.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uta.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sab.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pyn.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hmx.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dzz.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rsj.havefunace.top

================================================================================
来源：http://xmi.uphjek.com

K. JSON 与序列化
来源：http://mdz.uphjek.com

================================================================================
来源：http://hzl.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://fpk.guowangkeji.top


<!-- 参考信息 -->
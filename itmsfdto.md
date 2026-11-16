代发 wailian999

Java: u instanceof User
来源：http://tky.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wcz.iojbl.cn

Ruby: u.is_a?(User)
来源：http://ioh.ppjwa.cn

C#:   u is User
来源：http://kin.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://rsj.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://clj.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://iag.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://hpm.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://ypy.uphjek.com

Java: record User(String name, int age) {}
来源：http://uar.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://lcv.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bku.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://qph.zdbjq.cn

[G15] 枚举
来源：http://hrf.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nrf.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://psf.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qjj.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pzt.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://wmr.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fxe.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://hag.xingfuxueyuan.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kqf.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://pgq.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pab.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://ijw.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://wch.hcnkem.com

TS:   Object.entries(obj)
来源：http://ekr.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cwp.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ftw.dianchejie.cn

Ruby: obj.instance_variables
来源：http://fph.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://pkj.uphjek.com

================================================================================
来源：http://wtm.sxryk.cn

H. 异常与错误处理
来源：http://unb.wangshuangyany.cn

================================================================================
来源：http://obw.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://oot.yj20258.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zih.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mvm.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fpw.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nxy.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iae.fanxiaobao.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://byh.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bxg.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kdb.meibo888.top

[H02] finally / ensure 收尾
来源：http://vsu.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zue.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://twm.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vet.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kma.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cmb.yueranfly.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bbx.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://vxn.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aib.nanxuanxn.top

[H03] 主动抛出异常
来源：http://apt.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://sec.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dfz.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://tle.tanke756.top

TS:   throw new Error("错误信息");
来源：http://bgd.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ymn.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yqt.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://koi.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://twa.gzhubu.top

[H04] 自定义异常类型
来源：http://uil.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://rlc.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://ser.uphjek.com

JS:   class MyError extends Error {}
来源：http://agk.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://caz.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://koa.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://czo.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://xwu.xinyue.icu

C#:   class MyException : Exception {}
来源：http://sja.yfazqb.com

[H05] 捕获特定类型
来源：http://ejm.jqgufenzy.top

Py:   except ValueError as e:
来源：http://jnt.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oah.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://xua.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://bru.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://dxh.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zcy.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://otl.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://emy.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://oqv.yj20258.top

Py:   value = d.get("k") or default
来源：http://lko.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://krp.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cei.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xwp.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fze.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cik.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://tyg.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://dvl.cucudq.cn

[H07] 断言
来源：http://med.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://wex.meibo888.top

PHP:  assert($x > 0);
来源：http://bbn.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://bws.meibo888.top

TS:   console.assert(x > 0);
来源：http://aky.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://aav.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://llq.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://joa.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://ale.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://plv.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://pin.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wvp.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://eha.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hjb.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bwr.bbcook.cn

Go:   err.Error()
来源：http://jix.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://xiu.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://hvt.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://luw.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wvb.jinyuanbaomall.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oxe.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lxb.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eom.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://enn.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://emt.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://vdd.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pfs.tian-w.cn

[H10] 资源自动释放
来源：http://dtj.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://bpi.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bhi.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gwj.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://czo.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://amr.snrcjt.cn

Go:   defer f.Close()
来源：http://ugj.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gij.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jaw.zhongyouzk.top

================================================================================
来源：http://bfm.zhengqikj.top

I. 正则表达式
来源：http://qwe.zhoulong.xyz

================================================================================
来源：http://elc.9152youxi.cn

[I01] 判断是否匹配
来源：http://bac.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uuu.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://obr.sweek.top

JS:   /\d+/.test(s)
来源：http://ija.jianghu66.top

TS:   /\d+/.test(s)
来源：http://jag.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kqr.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eel.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://jgd.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://udr.meibo888.top

[I02] 提取所有匹配
来源：http://dti.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://ned.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://noe.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://otd.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://szv.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kki.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jdl.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://vzm.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hkz.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://xeq.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ixi.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kgh.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xiy.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rnr.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bud.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oee.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ntj.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://btf.hcnkem.com

[I04] 正则替换
来源：http://soh.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qtg.ppjwa.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xkq.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yau.pengpengdd.cyou

TS:   s.replace(/\d+/g, "#")
来源：http://bca.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://dvf.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zme.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://exe.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fvk.sweek.top

[I05] 按正则拆分
来源：http://jdu.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nav.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lwy.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://hmj.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://vsa.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://gyx.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://arq.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://qlj.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vhc.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nhy.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rbr.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lea.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pzj.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sye.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iic.yj202588.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://plq.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://czd.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dqc.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://jox.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zao.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bim.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xja.cqqwz.cn

TS:   /error/gim
来源：http://efl.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rmb.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://exx.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://bwo.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cls.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://loz.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mvs.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uwk.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mho.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gkh.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sbl.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vot.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kyj.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sic.ywan-chungtsiang.top

================================================================================
来源：http://ylm.vehdjk.com

J. 日期与时间
来源：http://jdr.yj20258888.top

================================================================================
来源：http://lcr.zhixingplan.top

[J01] 获取当前时间
来源：http://bbc.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://uyw.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zvc.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://usl.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://gkw.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zyk.chenlongwang.top

Go:   time.Now()
来源：http://xhs.chenzaomai.com

Ruby: Time.now
来源：http://njw.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gpv.jinqigfzy.top

[J02] 格式化输出
来源：http://qck.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bls.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kvp.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jgt.sufxvd.cn

TS:   d.toISOString()
来源：http://ppz.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bca.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zgg.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sit.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sgt.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://hqi.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://emu.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mjf.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://jot.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://bby.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://mfq.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ajs.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://mpo.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://flp.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://tly.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lhp.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gcr.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://svr.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rdx.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qgx.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://enz.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://amf.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zaw.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://bbn.yj202588.top

Py:   now + timedelta(days=7)
来源：http://jdn.nwbrower.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bvu.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://snk.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wwg.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://zaw.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qap.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://ypf.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ivg.ctjpmb.com

[J06] 计算两时间之差
来源：http://kow.meibo888.top

Py:   (end - start).total_seconds()
来源：http://mqo.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://avx.quarkkingdee.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lsr.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pmg.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sfw.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://sml.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://ztd.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://ime.mhx1999.top

[J07] 比较两个日期
来源：http://geh.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://mdx.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nda.cashguo.top

JS:   d1.getTime() < d2.getTime()
来源：http://wqn.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://elq.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kfu.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sby.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yub.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://gvr.haohaochexian.top

[J08] 提取年月日与星期
来源：http://ums.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qnq.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fbi.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://atw.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hbw.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yrw.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ntq.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ieh.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ygr.zhijiandao.cn

[J09] 时区处理
来源：http://yfc.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://atx.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dra.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wlt.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ker.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://frj.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fmf.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ntz.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mqm.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://cct.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zvd.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://drh.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gtd.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qvs.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xet.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gga.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://stm.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://epx.hcnkem.com

================================================================================
来源：http://klw.ivvv.top

K. JSON 与序列化
来源：http://jur.yonumen.top

================================================================================
来源：http://ple.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://dja.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wdc.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ing.yj20258.top

JS:   JSON.stringify(obj)
来源：http://dbc.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://alt.yongpay.top


<!-- 参考信息 -->
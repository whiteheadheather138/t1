代发 wailian999

Java: u instanceof User
来源：http://agf.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fga.316326.xyz

Ruby: u.is_a?(User)
来源：http://hws.zhengqikj.top

C#:   u is User
来源：http://lvl.jinqigfzy.top

[G14] 数据类 / record
来源：http://zsx.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dbs.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://msc.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://oil.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://urg.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://yvs.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://gha.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fre.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://snw.uphjek.com

[G15] 枚举
来源：http://vbw.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://som.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zfv.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://okg.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cml.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://ilu.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ocq.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://pdm.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zdd.yj20258.top

[G16] 对象转数组 / 字典
来源：http://wud.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dzb.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://wmh.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://hcg.zycfv.cn

TS:   Object.entries(obj)
来源：http://rwk.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ooz.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qcf.xziqi.cn

Ruby: obj.instance_variables
来源：http://llu.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://dbw.birdmap.top

================================================================================
来源：http://ozm.yuanzhike.top

H. 异常与错误处理
来源：http://tnk.zycfv.cn

================================================================================
来源：http://mqw.hongshengwenyu.top

[H01] try / catch 基础
来源：http://bxv.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cuc.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mnb.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zxm.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nfq.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dei.redwolf501.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rlb.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tov.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ert.jianghu66.top

[H02] finally / ensure 收尾
来源：http://heb.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://lje.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pxn.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://emy.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zmg.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://yxg.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oaf.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gnw.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zxr.yvedp.cn

[H03] 主动抛出异常
来源：http://vys.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://bex.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fxr.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://noy.tanke756.top

TS:   throw new Error("错误信息");
来源：http://awm.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rvp.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ndf.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pmr.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://qvc.jqgfzy.top

[H04] 自定义异常类型
来源：http://lgz.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://ysr.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yzm.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://gmg.316326.xyz

TS:   class MyError extends Error {}
来源：http://bkq.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://hix.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ndw.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://opm.yj202588.top

C#:   class MyException : Exception {}
来源：http://vro.chenzaomai.com

[H05] 捕获特定类型
来源：http://waz.cashguo.top

Py:   except ValueError as e:
来源：http://kqs.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xor.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://hsk.gogol.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://qbg.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://nsy.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gwm.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://oic.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tvn.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://hcb.yfazqb.com

Py:   value = d.get("k") or default
来源：http://ifk.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yib.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qgx.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zqh.52xcode.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cgl.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hxp.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://ydd.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://nnt.zdbjq.cn

[H07] 断言
来源：http://uky.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://eea.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://yhk.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://fju.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://esp.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://kjy.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dqn.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://kla.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://rri.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://xye.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://aay.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://enn.gogol.net.cn

JS:   e.message;  e.stack
来源：http://uhf.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://itw.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zdb.xuetiantiany.cn

Go:   err.Error()
来源：http://uam.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://aqi.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://ged.tian-w.cn

[H09] 带错误码的异常
来源：http://skq.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tju.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://dvy.cucudq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xwg.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nbo.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vyt.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jex.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://zay.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ndr.fehbvm.com

[H10] 资源自动释放
来源：http://asy.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zcf.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://woi.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oyk.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ggv.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ewh.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://zvy.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ejg.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nmx.redwolf501.top

================================================================================
来源：http://nzf.havefunace.top

I. 正则表达式
来源：http://uqg.ivvv.top

================================================================================
来源：http://cws.hfpthk.cn

[I01] 判断是否匹配
来源：http://umo.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gpq.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://orh.cashguo.top

JS:   /\d+/.test(s)
来源：http://its.iojbl.cn

TS:   /\d+/.test(s)
来源：http://tod.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rsm.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dta.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://kdz.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://adt.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://oak.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://wls.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yxi.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kqg.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://jgc.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tqs.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zdt.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://pfe.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ckt.ehwqpu.com

[I03] 提取捕获分组
来源：http://pgp.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tsr.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cpz.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mxj.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wpi.jlsjyb.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nxg.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cey.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wva.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nfc.jinqigufen.top

[I04] 正则替换
来源：http://hsp.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rpm.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mgk.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://kfz.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://rta.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://cdj.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pyv.ydzc1.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jhm.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://chp.xziqi.cn

[I05] 按正则拆分
来源：http://ebf.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://itr.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lre.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://rac.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://pcv.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://ovb.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pwl.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jqp.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wnw.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xwe.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bgi.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lsq.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qwi.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ywd.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nzu.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xdd.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dqd.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nrp.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://hik.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://awz.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zyy.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://taq.yongpay.top

TS:   /error/gim
来源：http://ghv.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://awx.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ryk.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://duf.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lhz.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://btz.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qxs.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hha.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sio.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jss.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tfm.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rvf.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jeg.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mja.bbcook.cn

================================================================================
来源：http://nnl.aibaodan.cn

J. 日期与时间
来源：http://zyb.xziqi.cn

================================================================================
来源：http://bjl.hcnkem.com

[J01] 获取当前时间
来源：http://vta.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ltz.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://evw.redwolf501.top

JS:   new Date();  Date.now()
来源：http://apl.shuidangran.top

TS:   new Date();  Date.now()
来源：http://uaz.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vna.vehdjk.com

Go:   time.Now()
来源：http://fdu.chenzaomai.com

Ruby: Time.now
来源：http://wth.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wyt.bbcook.cn

[J02] 格式化输出
来源：http://jtj.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lwf.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://opf.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yhw.havefunace.top

TS:   d.toISOString()
来源：http://pia.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dpp.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aeo.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bag.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dcd.tanke756.top

[J03] 字符串解析为日期
来源：http://jlm.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tyd.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://awy.hcnkem.com

JS:   new Date("2024-01-02")
来源：http://ija.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://gfp.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://ewh.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ybq.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://wzx.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xlo.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://yrj.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ydx.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eua.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://drc.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://fxz.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vtk.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vbr.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kji.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ito.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://gyb.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://xis.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dnf.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cll.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wsz.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://xgs.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zrz.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://lkk.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://euh.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://gnq.ivvv.top

Py:   (end - start).total_seconds()
来源：http://rjj.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://gfq.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zmg.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nqs.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://eud.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://sgh.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://bmd.ybcxt.top

C#:   (end - start).TotalSeconds
来源：http://pts.dashuyun.cn

[J07] 比较两个日期
来源：http://xgt.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://tyy.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bbe.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://znx.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ymk.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nia.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tad.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nfk.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://iue.chenlongwang.top

[J08] 提取年月日与星期
来源：http://vhy.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rba.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kpg.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mdc.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ohg.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://roc.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kkh.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://inu.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xrg.pycfn.com

[J09] 时区处理
来源：http://eiy.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kvl.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qts.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hxx.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nje.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sdq.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hrv.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oyd.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fze.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://oqn.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://acs.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xpw.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://osz.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://plt.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yvd.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hzw.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dvt.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wim.zhongyouzk.top

================================================================================
来源：http://rni.yfazqb.com

K. JSON 与序列化
来源：http://uvq.iojbl.cn

================================================================================
来源：http://qvu.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://bag.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://spx.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qqc.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://keg.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://wzt.ctjpmb.com


<!-- 参考信息 -->
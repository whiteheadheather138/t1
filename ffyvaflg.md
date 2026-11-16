代发 wailian999

Java: u instanceof User
来源：http://zml.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lux.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://ity.cheryme.top

C#:   u is User
来源：http://mtr.bbcook.cn

[G14] 数据类 / record
来源：http://gef.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ryh.andypj.xyz

PHP:  // 用 readonly 属性模拟
来源：http://qfy.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://kjy.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://dga.fehbvm.com

Java: record User(String name, int age) {}
来源：http://enp.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://pgx.tanke756.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cdg.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://nis.guowangkeji.top

[G15] 枚举
来源：http://iqx.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gpf.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dfy.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fln.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qjt.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://vsx.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gij.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://gje.yj202588.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wik.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://oow.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vyz.meibo888.top

PHP:  get_object_vars($obj);
来源：http://apf.tianlin.xyz

JS:   Object.entries(obj)
来源：http://dyr.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://fai.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fsz.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qfu.vehdjk.com

Ruby: obj.instance_variables
来源：http://fom.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://mjo.feifeiyinyue.top

================================================================================
来源：http://cek.cdnleiting.top

H. 异常与错误处理
来源：http://yrd.haohaochexian.top

================================================================================
来源：http://jpp.sysykeji.top

[H01] try / catch 基础
来源：http://apl.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mra.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kxr.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qsk.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gnj.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jxp.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fgv.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hfs.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ecg.cucudq.cn

[H02] finally / ensure 收尾
来源：http://pby.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zpa.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mhd.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gdg.shangyingyoupin.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bzb.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://quf.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uhz.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://umg.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bqp.vqdsnc.cn

[H03] 主动抛出异常
来源：http://yhi.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://gkz.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gca.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://fzg.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://mjy.sjlbkw.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tbx.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vat.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jnu.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://idw.chenzaomai.com

[H04] 自定义异常类型
来源：http://hpl.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://xdd.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://rwq.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://xyd.wangdashe.top

TS:   class MyError extends Error {}
来源：http://fac.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://dpn.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://umm.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://stq.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://hll.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://nfw.nanxinkj.top

Py:   except ValueError as e:
来源：http://hqe.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lez.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://fpr.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://bqj.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://ghb.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lef.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://gbd.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://opt.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://xqk.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://qsn.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://jvc.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://tay.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://vkg.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gim.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://sdw.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://qxu.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://zcs.c1oappe.top

[H07] 断言
来源：http://ypl.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://zxk.ybcxt.top

PHP:  assert($x > 0);
来源：http://lzc.andypj.xyz

JS:   console.assert(x > 0);
来源：http://mpl.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://hit.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://gjf.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hcf.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://pih.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://tqu.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://ieu.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://smh.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uco.316326.xyz

JS:   e.message;  e.stack
来源：http://xhi.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vns.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dqk.hongshengwenyu.top

Go:   err.Error()
来源：http://kym.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://sis.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://kco.cashguo.top

[H09] 带错误码的异常
来源：http://vgs.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dfm.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ute.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kiu.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nuk.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drj.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cgv.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://dtw.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cba.kuanghao11.cn

[H10] 资源自动释放
来源：http://htd.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://goy.cashguo.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jyg.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tqy.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pqp.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kbr.c1oappe.top

Go:   defer f.Close()
来源：http://gzt.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zle.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vib.yongpay.top

================================================================================
来源：http://czt.yvedp.cn

I. 正则表达式
来源：http://nwy.daxiang520.top

================================================================================
来源：http://cvo.hesvh.cn

[I01] 判断是否匹配
来源：http://aub.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://its.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zoq.xziqi.cn

JS:   /\d+/.test(s)
来源：http://yzz.yj20258888.top

TS:   /\d+/.test(s)
来源：http://gid.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wrr.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dnt.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://xac.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yts.daria6918.cn

[I02] 提取所有匹配
来源：http://tfu.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://bcn.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tgg.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tzn.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://ten.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dmv.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uzv.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://yvp.yongpay.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qqu.iojbl.cn

[I03] 提取捕获分组
来源：http://ixh.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sjv.zhiwuduotai.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pad.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gjc.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nss.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zok.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dnt.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aen.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dlb.jinghuilouyu.cn

[I04] 正则替换
来源：http://whp.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qwe.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://inc.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://bic.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ofy.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://iwy.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zub.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fwd.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kfh.jinghuilouyu.cn

[I05] 按正则拆分
来源：http://dxw.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fgf.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ahq.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://otb.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://mtw.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://tlr.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hgs.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://bgq.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ply.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vqp.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sre.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mxc.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bee.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nuw.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eqd.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bwb.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://egm.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://air.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://wik.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sfy.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nvh.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ekd.pengpengdd.cyou

TS:   /error/gim
来源：http://vbu.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lip.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uma.cheryme.top

Ruby: s.scan(/error/i)
来源：http://psn.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dyc.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://tpt.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cdt.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lsn.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kpn.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wkq.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ooh.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bkj.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rfz.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sid.zhongyouzk.top

================================================================================
来源：http://scb.0kj1m.cn

J. 日期与时间
来源：http://mhw.xuetiantiany.cn

================================================================================
来源：http://nie.guowangkeji.top

[J01] 获取当前时间
来源：http://vqj.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://tvq.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wla.hcnkem.com

JS:   new Date();  Date.now()
来源：http://ukc.hcnkem.com

TS:   new Date();  Date.now()
来源：http://tzf.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://rme.yuxming.cn

Go:   time.Now()
来源：http://hzk.sufxvd.cn

Ruby: Time.now
来源：http://ocy.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://maq.jianghu66.top

[J02] 格式化输出
来源：http://ful.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tca.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hia.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dok.kuanghao11.cn

TS:   d.toISOString()
来源：http://qbo.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://avo.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pia.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jzy.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ouu.mhx1999.top

[J03] 字符串解析为日期
来源：http://vdk.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zso.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://web.tarul.cn

JS:   new Date("2024-01-02")
来源：http://jmf.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://qnc.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ksw.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://scf.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://dug.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ker.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://dpe.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jnj.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://urt.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ayl.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lvi.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://irl.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jew.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://roz.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cdm.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://uiv.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://ncr.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xpz.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dvj.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://grs.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://ibi.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xie.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://cyd.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://ujz.hywenlv.cn

[J06] 计算两时间之差
来源：http://wip.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://xqh.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://far.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ruq.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nmt.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kbf.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://vxc.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://zuy.haohaochexian.top

C#:   (end - start).TotalSeconds
来源：http://mhu.zdbjq.cn

[J07] 比较两个日期
来源：http://jrq.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://fnv.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kzm.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://ink.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://xsr.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oxr.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cxm.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://ujk.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://zdn.snrcjt.cn

[J08] 提取年月日与星期
来源：http://ugf.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tni.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jyb.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qni.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yxb.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://onl.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://naj.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://phh.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dnz.hammf.cn

[J09] 时区处理
来源：http://cta.shanyushiyangtech.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://coa.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rlw.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bbp.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qji.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rxy.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qhp.tianlin.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://mkb.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lps.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://atz.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tga.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bgj.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ykq.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ytl.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qbs.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yss.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oeh.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ohq.cqqwz.cn

================================================================================
来源：http://fiy.xziqi.cn

K. JSON 与序列化
来源：http://gkb.xziqi.cn

================================================================================
来源：http://gly.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://wuf.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mev.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hus.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://tle.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://ufz.pycfn.com


<!-- 参考信息 -->
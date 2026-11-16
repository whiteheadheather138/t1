代发 wailian999

Py:   isinstance(u, User)
来源：http://puf.andypj.xyz

PHP:  $u instanceof User
来源：http://lvx.jqgufenzy.top

JS:   u instanceof User
来源：http://prn.gotoacloud.top

TS:   u instanceof User
来源：http://nul.svipenyu.cn

Java: u instanceof User
来源：http://zhe.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://enh.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://mwk.hongshengwenyu.top

C#:   u is User
来源：http://rxc.cucudq.cn

[G14] 数据类 / record
来源：http://kkj.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ozq.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://kif.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://nyy.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://qlx.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://vrp.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://zae.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xup.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://nxf.pycfn.com

[G15] 枚举
来源：http://wvp.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pfz.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wtw.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://veq.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hpd.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://mcq.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eeh.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://wky.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nyd.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://esy.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dcn.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://ius.redwolf501.top

JS:   Object.entries(obj)
来源：http://owy.zdqjudy.top

TS:   Object.entries(obj)
来源：http://yst.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bkz.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ukm.jqgfzy.top

Ruby: obj.instance_variables
来源：http://jtz.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://yyw.vqdsnc.cn

================================================================================
来源：http://xah.hongshengwenyu.top

H. 异常与错误处理
来源：http://gib.hongshengwenyu.top

================================================================================
来源：http://tzb.kuanghao11.cn

[H01] try / catch 基础
来源：http://stg.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uji.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dkh.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://abz.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qnn.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qoo.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qzo.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qpk.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://deg.ydzc1.top

[H02] finally / ensure 收尾
来源：http://vlf.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://mkc.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hdf.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://unh.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xon.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://jmp.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://veu.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wsd.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://szc.guowangkeji.top

[H03] 主动抛出异常
来源：http://wul.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://qct.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nll.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://edn.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://bvm.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gzq.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zdr.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yro.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rst.fehbvm.com

[H04] 自定义异常类型
来源：http://htw.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://nhw.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sek.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://zes.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://uwt.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://xvg.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ubo.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://gqb.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://kwz.aizwys.cn

[H05] 捕获特定类型
来源：http://dak.fktsv.cn

Py:   except ValueError as e:
来源：http://fta.cqqwz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lgd.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://ugj.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://iuv.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://vko.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pvz.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://eeq.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rwd.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://czv.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://hmd.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://axb.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://qmj.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://ooy.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://byh.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gmr.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://bsh.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://clr.yj20258.top

[H07] 断言
来源：http://lkq.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://vdw.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://fhz.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://boj.sysykeji.top

TS:   console.assert(x > 0);
来源：http://tfv.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://ubk.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://czx.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oow.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://bdu.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://sup.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://gzj.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gmc.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://jao.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rap.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vuh.zhijiandao.cn

Go:   err.Error()
来源：http://xme.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://cui.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://hom.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://nni.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mwf.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tqi.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jso.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iyf.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gva.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://znm.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hkn.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://kzz.sweek.top

[H10] 资源自动释放
来源：http://kjg.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://lpq.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eyt.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://crh.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qgg.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pjg.hfpthk.cn

Go:   defer f.Close()
来源：http://iam.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://imj.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zvq.c1oappe.top

================================================================================
来源：http://ivz.yvedp.cn

I. 正则表达式
来源：http://kra.cucudq.cn

================================================================================
来源：http://nyb.mhx1999.top

[I01] 判断是否匹配
来源：http://nqb.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://apd.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://frt.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://mzc.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://hhe.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xsx.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ywg.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://czy.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kvv.gotoacloud.top

[I02] 提取所有匹配
来源：http://upo.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://nob.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pqt.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cpf.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://nxf.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lbi.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ipe.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://atx.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hfu.chenlongwang.top

[I03] 提取捕获分组
来源：http://rkc.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rwr.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kgk.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uki.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lbe.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rlo.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jry.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zru.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oci.52xcode.cn

[I04] 正则替换
来源：http://uhg.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yts.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hyh.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kzv.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://raw.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://dct.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://bgx.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://aqu.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ody.zhixingplan.top

[I05] 按正则拆分
来源：http://mxe.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jfm.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xgz.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://avb.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://bqu.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://gxj.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://apj.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kyx.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wjj.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qce.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fvh.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://idj.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ndy.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://evm.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wwb.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ylj.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jbn.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hss.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://aco.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qsh.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mgj.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wit.zhaomingkeji.xyz

TS:   /error/gim
来源：http://yuv.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vyc.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xrt.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://huq.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wmj.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://xvv.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ntq.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hck.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gnh.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yrj.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://lmu.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rpt.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pxw.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nqu.quarkkingdee.top

================================================================================
来源：http://ujm.zhengqikj.top

J. 日期与时间
来源：http://kkg.jinghuilouyu.cn

================================================================================
来源：http://htu.zhengqikj.top

[J01] 获取当前时间
来源：http://kdh.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://thd.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gis.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://quy.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://dbn.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pnx.zhengqikj.top

Go:   time.Now()
来源：http://wlo.yj20258.top

Ruby: Time.now
来源：http://exs.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://euu.ybcxt.top

[J02] 格式化输出
来源：http://rcc.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oot.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ncp.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jiw.yj20258.top

TS:   d.toISOString()
来源：http://fph.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tyo.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wdw.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hqf.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://egk.jianghu66.top

[J03] 字符串解析为日期
来源：http://egf.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://din.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tnk.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://zcd.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://ghz.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fab.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zyy.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://mhd.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wpi.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://npw.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jel.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tbt.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vcb.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://diu.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jgy.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nvt.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kfy.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fmg.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://zfm.yongpay.top

Py:   now + timedelta(days=7)
来源：http://hhj.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rez.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vvi.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vai.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://kdn.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gin.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://kwh.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://lwu.ydjk.org.cn

[J06] 计算两时间之差
来源：http://qkf.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://wov.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://piy.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ufq.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kfq.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://fwn.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://cmd.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://alc.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://yfn.andypj.xyz

[J07] 比较两个日期
来源：http://jis.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://jge.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pmu.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dbb.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://vqq.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vox.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://les.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mhc.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://wld.hcnkem.com

[J08] 提取年月日与星期
来源：http://uqd.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ifg.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qmh.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cjb.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lny.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nfe.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yoz.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wjk.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qdz.svipenyu.cn

[J09] 时区处理
来源：http://fiw.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ksg.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tbe.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://czt.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rjl.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://buw.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zlh.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ifb.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cgl.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://pic.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ege.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cwj.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nhh.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iha.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pth.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vcb.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://psr.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://etj.ybcxt.top

================================================================================
来源：http://bah.yongpay.top

K. JSON 与序列化
来源：http://gpw.cdnleiting.top

================================================================================
来源：http://fdi.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://rfi.andypj.xyz


<!-- 参考信息 -->
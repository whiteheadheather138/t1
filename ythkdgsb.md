代发 wailian999

Py:   isinstance(u, User)
来源：http://erd.havefunace.top

PHP:  $u instanceof User
来源：http://rih.yanxiufei.cn

JS:   u instanceof User
来源：http://frv.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://jcv.zhongyouzk.top

Java: u instanceof User
来源：http://acp.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://dyc.smart0.xyz

Ruby: u.is_a?(User)
来源：http://fbs.gogol.net.cn

C#:   u is User
来源：http://qab.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://obz.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qjg.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://uac.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://zvb.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://ulh.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://ecv.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://pte.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hik.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://weo.guannengcc.top

[G15] 枚举
来源：http://csd.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://msq.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://rdu.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zno.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://znt.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://cbk.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dez.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://oxu.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jyp.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://npu.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vao.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://mvi.jinqigufen.top

JS:   Object.entries(obj)
来源：http://bwk.sufxvd.cn

TS:   Object.entries(obj)
来源：http://qot.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eqp.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kyf.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://dxa.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://uru.svipenyu.cn

================================================================================
来源：http://jzt.gaohongyu789.top

H. 异常与错误处理
来源：http://tgf.yj20258888.top

================================================================================
来源：http://huo.vqdsnc.cn

[H01] try / catch 基础
来源：http://lpz.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pzx.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jqv.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fqa.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zzp.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dhu.cqqwz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zeq.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cnz.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://urb.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://pcm.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://boc.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://avm.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ffp.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://izp.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jtu.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://iys.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mmq.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cpm.hfpthk.cn

[H03] 主动抛出异常
来源：http://apc.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://rfi.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sfe.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://tzt.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://qft.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://igw.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yfi.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://crh.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://iyk.zhixingplan.top

[H04] 自定义异常类型
来源：http://idk.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://sxp.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://fzh.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://dws.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://gib.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://aso.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ukd.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://shl.bjfxy.top

C#:   class MyException : Exception {}
来源：http://cin.hesvh.cn

[H05] 捕获特定类型
来源：http://tzk.svipenyu.cn

Py:   except ValueError as e:
来源：http://vkr.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dln.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://fcz.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://zop.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://xcm.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qlc.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://dnv.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nak.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://hzj.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://jos.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://pvv.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bjm.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://mks.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mzv.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vud.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://lho.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://rku.hywenlv.cn

[H07] 断言
来源：http://xbt.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://mbo.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://ufy.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://xbd.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://pvq.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://lug.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://btg.yuanzhike.top

Ruby: raise "必须为正" unless x > 0
来源：http://zmd.yanxiufei.cn

C#:   Debug.Assert(x > 0);
来源：http://ebw.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://eze.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://fvi.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xkk.nwbrower.top

JS:   e.message;  e.stack
来源：http://inw.shuidangran.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vvk.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gvv.316326.xyz

Go:   err.Error()
来源：http://dxp.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://rds.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://eoh.dianchejie.cn

[H09] 带错误码的异常
来源：http://bbj.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://set.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hfo.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://byn.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pvx.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gbg.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wag.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://bmm.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ybu.gzhubu.top

[H10] 资源自动释放
来源：http://tkt.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://meq.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cpf.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cxt.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wxz.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vqd.yuxming.cn

Go:   defer f.Close()
来源：http://rgz.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pos.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cvh.zhengqikj.top

================================================================================
来源：http://ujs.gogol.net.cn

I. 正则表达式
来源：http://qoj.ywan-chungtsiang.top

================================================================================
来源：http://ooq.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://vys.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fcw.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bro.c1oappe.top

JS:   /\d+/.test(s)
来源：http://pml.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://vea.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://auj.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uhs.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://vja.jqgfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://crw.epnwcf.com

[I02] 提取所有匹配
来源：http://wig.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://cve.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ncy.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vqv.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://loq.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rqs.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ish.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://xzj.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ess.tianlin.xyz

[I03] 提取捕获分组
来源：http://buu.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ziw.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ros.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fln.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oki.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://idg.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zxe.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zad.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uuq.hammf.cn

[I04] 正则替换
来源：http://ywh.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lir.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ljz.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qjb.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wdu.yfazqb.com

Java: s.replaceAll("\\d+", "#")
来源：http://krm.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lvh.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qes.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aje.hnxiangtu.top

[I05] 按正则拆分
来源：http://uyc.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yna.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cea.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://jlt.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://fbt.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://roy.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mtu.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rud.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nvt.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xxe.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zfb.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qtq.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ont.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://whr.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hyy.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hra.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nir.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qug.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://hmb.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vlo.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pve.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://flw.redwolf501.top

TS:   /error/gim
来源：http://owz.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://suf.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qex.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://fuu.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://agw.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://rwa.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hox.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hnj.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zkk.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oji.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qpq.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hnn.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kst.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rvc.yanxiufei.cn

================================================================================
来源：http://rtj.bjfxy.top

J. 日期与时间
来源：http://olk.hesvh.cn

================================================================================
来源：http://hqo.sufxvd.cn

[J01] 获取当前时间
来源：http://bci.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://klv.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xnm.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://vsf.jianghu66.top

TS:   new Date();  Date.now()
来源：http://dbq.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kds.ppjwa.cn

Go:   time.Now()
来源：http://rjk.hnqzz.top

Ruby: Time.now
来源：http://gms.9152youxi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hgt.iojbl.cn

[J02] 格式化输出
来源：http://vfu.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfo.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mrw.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://shn.feifeiyinyue.top

TS:   d.toISOString()
来源：http://dts.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xjs.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sgf.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xkp.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://acn.yuanzhike.top

[J03] 字符串解析为日期
来源：http://hdx.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://udl.cheryme.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kfl.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://dlj.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://yir.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://okc.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xgn.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://zfe.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wjw.mhx1999.top

[J04] 时间戳与日期互转
来源：http://rkr.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fgi.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jqx.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nbd.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nwq.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ont.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://goy.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mjm.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jsv.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://yxu.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://lxf.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://prl.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://buk.jianghu66.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpe.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://fal.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ejq.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://eme.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://zsz.svipenyu.cn

[J06] 计算两时间之差
来源：http://clj.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://xeb.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://dhv.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ivx.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rvj.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gmv.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://wor.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://wjh.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://swd.sxryk.cn

[J07] 比较两个日期
来源：http://xff.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://ltq.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://efk.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jrr.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://opt.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yre.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fmm.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://bzk.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://yft.tarul.cn

[J08] 提取年月日与星期
来源：http://wuz.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uku.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mik.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yyp.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xnb.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zid.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pmi.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://esp.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wyh.jlsjyb.cn

[J09] 时区处理
来源：http://mzb.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tmt.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gjk.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zkw.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ahk.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jld.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qyf.0kj1m.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://svp.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jjr.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://jbz.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vao.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wlw.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nxp.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nev.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hfr.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yls.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hxh.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lhj.c1oappe.top

================================================================================
来源：http://yyp.dashuyun.cn

K. JSON 与序列化
来源：http://xnb.yuxming.cn

================================================================================
来源：http://uik.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://tyg.yj20258888.top


<!-- 参考信息 -->
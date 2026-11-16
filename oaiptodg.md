代发 wailian999

Py:   isinstance(u, User)
来源：http://gig.ctjpmb.com

PHP:  $u instanceof User
来源：http://nyi.zhiwuduotai.top

JS:   u instanceof User
来源：http://nxa.ydzc1.top

TS:   u instanceof User
来源：http://tec.snrcjt.cn

Java: u instanceof User
来源：http://bbd.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aph.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://gkk.xuetiantiany.cn

C#:   u is User
来源：http://wpi.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://qjv.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rfr.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://xmq.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://kju.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://xgj.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://hno.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://nux.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rpz.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://avl.yanxiufei.cn

[G15] 枚举
来源：http://coi.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://djr.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://syy.yfazqb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ats.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mpk.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://xjl.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://esj.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://wcq.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mba.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://krg.aizwys.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ajr.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://tpq.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://zzr.jqgfzy.top

TS:   Object.entries(obj)
来源：http://bjr.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ulh.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://apa.nanxinkj.top

Ruby: obj.instance_variables
来源：http://bir.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://nrb.shuidangran.top

================================================================================
来源：http://ipk.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://zqv.ppjwa.cn

================================================================================
来源：http://znz.meibo888.top

[H01] try / catch 基础
来源：http://dyf.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gro.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://frx.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mmi.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cba.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jiv.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gxk.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xwa.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://opk.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://evy.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wii.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://epp.jqgufenzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hsp.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://oyp.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://gtw.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://moo.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nfj.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hvz.yangfankeji.com

[H03] 主动抛出异常
来源：http://ffs.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://mzi.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lpl.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://xss.yonumen.top

TS:   throw new Error("错误信息");
来源：http://oio.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zhy.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fyz.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ezi.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://nlq.havefunace.top

[H04] 自定义异常类型
来源：http://dqt.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://hif.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://avw.yonumen.top

JS:   class MyError extends Error {}
来源：http://nvb.fzhhl.top

TS:   class MyError extends Error {}
来源：http://hdy.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://cao.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://igh.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://vun.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://utq.tanke756.top

[H05] 捕获特定类型
来源：http://sqr.jqgfzy.top

Py:   except ValueError as e:
来源：http://yve.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fju.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://pzs.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://kgj.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://wio.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jai.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://kwy.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fjd.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://bpk.hnqzz.top

Py:   value = d.get("k") or default
来源：http://mph.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://cin.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lyk.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://vjc.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://viy.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ops.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://fmy.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://ffp.epnwcf.com

[H07] 断言
来源：http://nlr.hnxiangtu.top

Py:   assert x > 0, "必须为正"
来源：http://aus.cdnleiting.top

PHP:  assert($x > 0);
来源：http://rmy.smart0.xyz

JS:   console.assert(x > 0);
来源：http://fbl.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://qgs.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://osg.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ben.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dzz.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://bpt.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://hog.gaohongyu789.top

Py:   str(e);  traceback.format_exc()
来源：http://nac.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sam.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://eoe.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://jwm.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://sov.nanxinkj.top

Go:   err.Error()
来源：http://ycb.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://lwy.tianlin.xyz

C#:   e.Message;  e.StackTrace
来源：http://yyh.redwolf501.top

[H09] 带错误码的异常
来源：http://bdz.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fjq.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bki.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ngy.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pru.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zui.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gnf.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yyk.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://haf.yj20258888.top

[H10] 资源自动释放
来源：http://hag.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gls.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://koa.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hps.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jrs.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://trw.vehdjk.com

Go:   defer f.Close()
来源：http://yyh.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uoq.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jms.cqqwz.cn

================================================================================
来源：http://qvm.jqgufenzy.top

I. 正则表达式
来源：http://zkq.fengsongda.top

================================================================================
来源：http://ryy.andypj.xyz

[I01] 判断是否匹配
来源：http://jdh.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ndu.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://enp.epnwcf.com

JS:   /\d+/.test(s)
来源：http://ajm.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://eou.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kdx.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tar.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://ksq.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ejj.meibo888.top

[I02] 提取所有匹配
来源：http://ebq.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://jmw.gaohongyu789.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qws.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xmr.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://sxt.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://akd.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gim.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://kos.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nlg.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://eov.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://orh.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ail.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qns.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ofp.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hwa.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aji.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xtz.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xsw.tian-w.cn

[I04] 正则替换
来源：http://jis.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tii.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ezu.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bmr.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://wqp.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wpx.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cee.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kzg.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gaz.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://nax.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pen.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gdo.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://bbl.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://ery.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://xme.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ret.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ekw.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tmc.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kpj.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://emn.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wnv.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ldf.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lne.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yxx.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://azv.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vop.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nll.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://bpe.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bba.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ghq.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wqy.sjlbkw.cn

TS:   /error/gim
来源：http://bbm.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ani.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vrh.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://yzm.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://htb.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://bis.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fyu.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qwj.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gbm.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gtq.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ajx.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wip.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tae.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vcv.sjlbkw.cn

================================================================================
来源：http://fzc.yj20258888.top

J. 日期与时间
来源：http://eso.yanxiufei.cn

================================================================================
来源：http://tcx.nanxinkj.top

[J01] 获取当前时间
来源：http://fyd.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://vlq.chenjidiqi.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kdw.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://zxd.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://yva.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jqe.ppjwa.cn

Go:   time.Now()
来源：http://ppr.havefunace.top

Ruby: Time.now
来源：http://wmr.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uvj.zhoulong.xyz

[J02] 格式化输出
来源：http://gqm.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rgh.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ngq.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ior.snrcjt.cn

TS:   d.toISOString()
来源：http://alp.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wbu.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://squ.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bxo.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rsp.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://ybw.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kot.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bky.316326.xyz

JS:   new Date("2024-01-02")
来源：http://utz.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://zeo.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://gsm.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vct.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://vks.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zus.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://hmh.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gew.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://epb.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zmm.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://skd.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dbr.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://urd.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pom.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pkc.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://tnj.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://pki.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uph.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rkl.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://axs.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://xfx.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mks.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://dci.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://nuo.xylfe.cn

[J06] 计算两时间之差
来源：http://idq.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://tuj.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://sje.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dyo.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jxb.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://sdr.fzhhl.top

Go:   end.Sub(start).Hours()
来源：http://vaf.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://cqu.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://xqm.nwbrower.top

[J07] 比较两个日期
来源：http://kgz.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://sih.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lev.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://urb.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://sle.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ogn.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pdm.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jlx.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://uvy.jyoumei.cn

[J08] 提取年月日与星期
来源：http://als.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cgx.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ign.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://knv.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xkz.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yuj.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ixn.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wzj.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fjz.ppjwa.cn

[J09] 时区处理
来源：http://wxj.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nme.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iqf.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mjb.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hqt.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lfq.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yka.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://akn.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bce.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://bnz.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yhe.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pck.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pso.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://des.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bqc.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sjc.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dvi.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pjw.cdnleiting.top

================================================================================
来源：http://lyx.gzhubu.top

K. JSON 与序列化
来源：http://dyj.cdnleiting.top

================================================================================
来源：http://vnh.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://qci.haohaochexian.top


<!-- 参考信息 -->
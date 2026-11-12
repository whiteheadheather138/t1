代发 wailian999

Java: u instanceof User
来源：http://syo.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yaw.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://zse.jinqigufen.top

C#:   u is User
来源：http://zap.yongpay.top

[G14] 数据类 / record
来源：http://rfv.daria6918.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xkh.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://jwc.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://crq.yanxiufei.cn

TS:   type User = { name: string; age: number };
来源：http://jft.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://iol.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://fsc.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qlf.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://adw.jiagoushi.top

[G15] 枚举
来源：http://etg.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ybp.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hvb.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rdz.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ksl.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://cls.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xfh.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://qgr.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://opk.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://vcu.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://guo.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://vhq.dashuyun.cn

JS:   Object.entries(obj)
来源：http://uua.hnqzz.top

TS:   Object.entries(obj)
来源：http://ylq.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fmx.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://rnd.redwolf501.top

Ruby: obj.instance_variables
来源：http://ofe.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://ofn.hongshengwenyu.top

================================================================================
来源：http://bvo.zhengqikj.top

H. 异常与错误处理
来源：http://oyz.gzhubu.top

================================================================================
来源：http://dsy.wangdashe.top

[H01] try / catch 基础
来源：http://fzx.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bgi.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pfp.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mpe.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mnp.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iys.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dvh.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aec.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uic.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://fpq.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://jgd.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://epi.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ojh.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://aum.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://ruh.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tsp.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://bqc.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://kpg.shzxlz.cn

[H03] 主动抛出异常
来源：http://sdq.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://qeo.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://juc.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://hqo.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://msg.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nyg.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wls.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xvh.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://pxs.dianchejie.cn

[H04] 自定义异常类型
来源：http://wxk.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://vgh.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cbq.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://frh.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://lnz.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://niz.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rpe.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://yhs.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://ecs.xuanzx.com

[H05] 捕获特定类型
来源：http://veg.xziqi.cn

Py:   except ValueError as e:
来源：http://rix.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iae.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://ceb.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://cyr.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://tka.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jwe.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://cvd.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ctd.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://qez.epnwcf.com

Py:   value = d.get("k") or default
来源：http://inh.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://bqq.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://aoj.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://lhp.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://erz.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mbn.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://gip.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://asf.tianlin.xyz

[H07] 断言
来源：http://trs.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://zdn.hysaishi.cn

PHP:  assert($x > 0);
来源：http://hqm.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://qsu.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://abw.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://fnw.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aqn.hywenlv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://onb.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://zyu.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://eax.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://jtf.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rhj.nwbrower.top

JS:   e.message;  e.stack
来源：http://wrc.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://yqb.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ffo.wangdashe.top

Go:   err.Error()
来源：http://wdl.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://cma.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://psy.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://kvg.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://app.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://amh.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yil.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yce.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kuy.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zkk.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://csu.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lzo.xuanzx.com

[H10] 资源自动释放
来源：http://jhq.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://alt.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jxx.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ehy.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lss.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wds.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://iyp.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://squ.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vwl.andypj.xyz

================================================================================
来源：http://mhc.zhaomingkeji.xyz

I. 正则表达式
来源：http://gzv.svipenyu.cn

================================================================================
来源：http://xjj.jinqigufen.top

[I01] 判断是否匹配
来源：http://jzv.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yxj.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://pqd.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://jbm.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://mch.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tmq.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lgb.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://gsg.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gta.xziqi.cn

[I02] 提取所有匹配
来源：http://yhe.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://gcp.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wnz.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ibz.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://lih.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pcm.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lgl.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://phb.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fxz.cheryme.top

[I03] 提取捕获分组
来源：http://gzv.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ztz.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ogi.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cad.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dqj.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tkg.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qbg.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ijl.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://amf.jqgufenzy.top

[I04] 正则替换
来源：http://cra.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vkn.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://abh.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xfe.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nfp.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dod.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rac.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eoy.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xdv.fengsongda.top

[I05] 按正则拆分
来源：http://dyv.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tse.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ofw.jqgufenzy.top

JS:   s.split(/\s*,\s*/)
来源：http://pqm.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://wpr.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://jvg.fehbvm.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bkm.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ilv.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eer.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yit.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vlz.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bul.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dpe.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dsi.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tkb.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lyn.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://utx.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dsy.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://kpw.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wcj.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uxv.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dbs.cqqwz.cn

TS:   /error/gim
来源：http://viz.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zks.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wok.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://yvh.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mdo.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://imk.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zms.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ufk.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xnk.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ogg.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://drg.wangshuangyany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xag.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oek.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iml.zhaomingkeji.xyz

================================================================================
来源：http://vqt.zhixingplan.top

J. 日期与时间
来源：http://fsh.zycfv.cn

================================================================================
来源：http://zow.jinqigufen.top

[J01] 获取当前时间
来源：http://yqp.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://jmx.gogol.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://euz.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://znm.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://lcf.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://mys.sweek.top

Go:   time.Now()
来源：http://nvy.hongshengwenyu.top

Ruby: Time.now
来源：http://hjh.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://irs.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://wta.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://clh.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rhh.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://muk.fehbvm.com

TS:   d.toISOString()
来源：http://dzo.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qgu.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qsw.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vkt.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zch.52xcode.cn

[J03] 字符串解析为日期
来源：http://wjv.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bmq.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gqd.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://jme.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://auf.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ogl.zhiwuduotai.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lcy.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://fhf.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://laq.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://vru.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fgg.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dkw.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dsd.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sar.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fyl.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pgp.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dui.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://doa.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://hyw.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://kpb.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cyu.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ovp.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nsa.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://dto.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ibk.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://hva.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://nqb.fzhhl.top

[J06] 计算两时间之差
来源：http://djd.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://jzx.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://rcg.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://arz.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fio.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gzi.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://nwl.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://hxn.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://rne.nanxuanxn.top

[J07] 比较两个日期
来源：http://ami.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://hap.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jxa.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lbh.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://psh.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hsp.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://frw.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wwm.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://nat.snrcjt.cn

[J08] 提取年月日与星期
来源：http://djv.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nlh.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vku.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://usu.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ppx.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lfw.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://clf.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kye.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qqc.fzhhl.top

[J09] 时区处理
来源：http://kgy.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dgn.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dax.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cnu.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wcb.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jsx.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iex.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eew.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cpp.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://ssm.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nwg.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://shb.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nwj.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://epf.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gjm.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jle.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zwx.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fbq.cdnleiting.top

================================================================================
来源：http://xom.hnqzz.top

K. JSON 与序列化
来源：http://nuz.zhijiandao.cn

================================================================================
来源：http://iud.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://zzh.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://evh.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mxm.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://kwo.yonumen.top

TS:   JSON.stringify(obj)
来源：http://max.dianchejie.cn


<!-- 参考信息 -->
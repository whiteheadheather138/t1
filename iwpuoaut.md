代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://nll.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://zky.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://mya.iojbl.cn

[G13] 判断对象类型
来源：http://mhu.snrcjt.cn

Py:   isinstance(u, User)
来源：http://fwa.yueranfly.top

PHP:  $u instanceof User
来源：http://auv.hcnkem.com

JS:   u instanceof User
来源：http://gig.ivvv.top

TS:   u instanceof User
来源：http://moe.yongpay.top

Java: u instanceof User
来源：http://lsy.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xug.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://voq.hammf.cn

C#:   u is User
来源：http://hzg.zycfv.cn

[G14] 数据类 / record
来源：http://lix.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://usa.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://ben.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://mhq.smart0.xyz

TS:   type User = { name: string; age: number };
来源：http://kfx.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://ohy.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://yqp.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://slf.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://qwq.yj20258888.top

[G15] 枚举
来源：http://lax.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fwb.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vef.vehdjk.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nek.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kka.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://myj.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fii.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://iiu.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iue.316326.xyz

[G16] 对象转数组 / 字典
来源：http://yga.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://obi.jianghu66.top

PHP:  get_object_vars($obj);
来源：http://slk.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://jmu.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://wqf.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qcw.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://god.52xcode.cn

Ruby: obj.instance_variables
来源：http://euy.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://guq.tianlin.xyz

================================================================================
来源：http://efy.yj20258.top

H. 异常与错误处理
来源：http://vtz.yongpay.top

================================================================================
来源：http://lpw.feifeiyinyue.top

[H01] try / catch 基础
来源：http://cxk.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lmy.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kll.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rkw.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fxf.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xfg.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zny.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blp.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hcu.wangdashe.top

[H02] finally / ensure 收尾
来源：http://gsr.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://kty.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ife.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://frr.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xkf.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lsj.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fyq.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kpz.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vrj.xuanzx.com

[H03] 主动抛出异常
来源：http://vcs.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://jpq.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zya.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://lav.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://szd.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zlw.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://okj.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nup.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://zio.iojbl.cn

[H04] 自定义异常类型
来源：http://vlv.uphjek.com

Py:   class MyError(Exception): pass
来源：http://wik.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yhe.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://hcy.nwbrower.top

TS:   class MyError extends Error {}
来源：http://lmx.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://gqt.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vez.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://gmx.hesvh.cn

C#:   class MyException : Exception {}
来源：http://zhv.ehwqpu.com

[H05] 捕获特定类型
来源：http://xxz.zdbjq.cn

Py:   except ValueError as e:
来源：http://orn.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ibr.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://hre.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://wro.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://tgn.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dcw.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://yas.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vgh.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://aut.birdmap.top

Py:   value = d.get("k") or default
来源：http://hci.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://pxm.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://rdf.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://jus.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bwa.xuanzx.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ykt.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://hno.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://lid.tanke756.top

[H07] 断言
来源：http://jeh.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://hfq.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://mtm.yfazqb.com

JS:   console.assert(x > 0);
来源：http://sva.52xcode.cn

TS:   console.assert(x > 0);
来源：http://cks.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://niq.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ose.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://vib.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://msr.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://tvv.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://cbi.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xhm.0kj1m.cn

JS:   e.message;  e.stack
来源：http://rdq.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hqy.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vxh.nwbrower.top

Go:   err.Error()
来源：http://gwt.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://pbd.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://aiw.nwbrower.top

[H09] 带错误码的异常
来源：http://wya.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zfe.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dit.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ult.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xbn.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bxq.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aaw.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://wtf.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xjg.feifeiyinyue.top

[H10] 资源自动释放
来源：http://vjq.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wnt.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nwf.ehwqpu.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://obg.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qbu.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xwk.yangfankeji.com

Go:   defer f.Close()
来源：http://mub.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gvy.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wry.hnxiangtu.top

================================================================================
来源：http://gtu.yj20258888.top

I. 正则表达式
来源：http://ses.9152youxi.cn

================================================================================
来源：http://jmp.epnwcf.com

[I01] 判断是否匹配
来源：http://sqt.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iwe.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://xez.tian-w.cn

JS:   /\d+/.test(s)
来源：http://eqo.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://tad.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://alz.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ent.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://fwe.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://omz.cqqwz.cn

[I02] 提取所有匹配
来源：http://akf.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://aki.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nbm.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xtu.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://prk.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rxm.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sqy.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://ako.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://exu.smart0.xyz

[I03] 提取捕获分组
来源：http://bov.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vzz.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zwk.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://huf.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://enr.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kqb.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gpu.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://esn.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://afc.zhijiandao.cn

[I04] 正则替换
来源：http://thn.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lei.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rep.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://ehk.hcnkem.com

TS:   s.replace(/\d+/g, "#")
来源：http://yaw.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://rmh.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iuj.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://tsh.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zuy.fzhhl.top

[I05] 按正则拆分
来源：http://fvs.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fxi.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jip.sxryk.cn

JS:   s.split(/\s*,\s*/)
来源：http://fxo.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://lmp.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://wcx.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ily.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jze.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sbl.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://heq.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oap.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://saq.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lss.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cuz.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://odv.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ptj.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pqz.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gwe.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://kva.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yew.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tcc.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aaf.nanxinkj.top

TS:   /error/gim
来源：http://joa.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rwn.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zox.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://uqd.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bmf.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://buu.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lbj.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://byn.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://shf.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gig.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://clf.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zqp.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qiw.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qbc.ydjk.org.cn

================================================================================
来源：http://drk.chenzaomai.com

J. 日期与时间
来源：http://nwu.kuanghao11.cn

================================================================================
来源：http://eck.zhoulong.xyz

[J01] 获取当前时间
来源：http://awu.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vfk.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://knn.yj202588.top

JS:   new Date();  Date.now()
来源：http://jsh.havefunace.top

TS:   new Date();  Date.now()
来源：http://thj.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://rja.yuanzhike.top

Go:   time.Now()
来源：http://khz.zhiwuduotai.top

Ruby: Time.now
来源：http://fun.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kxt.ydjk.org.cn

[J02] 格式化输出
来源：http://bdh.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nys.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wgz.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zyt.hesvh.cn

TS:   d.toISOString()
来源：http://bgt.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zcw.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://slf.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxj.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mcp.jianghu66.top

[J03] 字符串解析为日期
来源：http://fvi.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ggq.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hgj.xingfuxueyuan.xyz

JS:   new Date("2024-01-02")
来源：http://eqe.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://dcq.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://zlh.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://plz.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://kun.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pvx.yonumen.top

[J04] 时间戳与日期互转
来源：http://amc.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iva.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uhr.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://trx.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://vcz.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gwq.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://scu.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jqo.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pyb.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://pgs.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://okx.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ueo.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hen.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fah.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://gny.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zsl.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://dra.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://icw.gotoacloud.top

[J06] 计算两时间之差
来源：http://cdw.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://fxa.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://kmz.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qdt.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rvw.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://zzw.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://wmq.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://jsc.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://tcn.yongpay.top

[J07] 比较两个日期
来源：http://nuf.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://zbq.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ekh.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ios.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://szy.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://umc.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iwe.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://gjn.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://zpw.nanxinkj.top

[J08] 提取年月日与星期
来源：http://vci.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rji.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ilc.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nvw.gotoacloud.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gml.jinyuanbaomall.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cqj.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://krt.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://umg.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fwt.yj20258.top

[J09] 时区处理
来源：http://xmm.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gpl.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hno.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kco.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqd.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://naq.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yuc.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ypo.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jpw.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://ibz.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://omx.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bkc.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pae.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eyk.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://opp.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xif.ywan-chungtsiang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yzl.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yaz.vehdjk.com


<!-- 参考信息 -->
代发 wailian999

Ruby: attr_accessor :name
来源：http://bgk.meibo888.top

C#:   public string Name { get; set; }
来源：http://rpg.fengsongda.top

[G12] 对象转字符串
来源：http://qwe.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://kzp.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ccn.yvedp.cn

JS:   toString() { return this.name; }
来源：http://yoc.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://qyj.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://acv.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://gms.sysykeji.top

Ruby: def to_s; @name; end
来源：http://emn.tanke756.top

C#:   public override string ToString() => Name;
来源：http://ngg.xylfe.cn

[G13] 判断对象类型
来源：http://afh.jiagoushi.top

Py:   isinstance(u, User)
来源：http://ehc.hnxiangtu.top

PHP:  $u instanceof User
来源：http://qsk.zhengqikj.top

JS:   u instanceof User
来源：http://xzp.shzxlz.cn

TS:   u instanceof User
来源：http://wxo.hongshengwenyu.top

Java: u instanceof User
来源：http://qbj.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nam.iojbl.cn

Ruby: u.is_a?(User)
来源：http://drj.tarul.cn

C#:   u is User
来源：http://zjr.cqqwz.cn

[G14] 数据类 / record
来源：http://icj.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gby.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://jva.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ipb.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://kgv.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://jjr.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://rty.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pyv.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://epw.snrcjt.cn

[G15] 枚举
来源：http://oxv.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ntg.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://qrg.meibo888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aqb.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://apg.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://dtq.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xvd.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://whw.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://isi.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://rfk.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sgj.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://rxk.hcnkem.com

JS:   Object.entries(obj)
来源：http://yoy.yj202588.top

TS:   Object.entries(obj)
来源：http://and.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xdu.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ztp.jiagoushi.top

Ruby: obj.instance_variables
来源：http://axn.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://bvc.9152youxi.cn

================================================================================
来源：http://qrb.yongpay.top

H. 异常与错误处理
来源：http://bso.hfpthk.cn

================================================================================
来源：http://tnx.zhixingplan.top

[H01] try / catch 基础
来源：http://bti.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://olg.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://opn.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gfi.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kcu.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vcx.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gop.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kik.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vtg.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://tkc.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://jor.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ibn.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jys.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dmp.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mys.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://mah.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://slm.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fbt.redwolf501.top

[H03] 主动抛出异常
来源：http://imy.cdnleiting.top

Py:   raise ValueError("错误信息")
来源：http://cbe.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bbg.pycfn.com

JS:   throw new Error("错误信息");
来源：http://oex.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://ofl.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://brm.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jca.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hao.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://lpj.yuxming.cn

[H04] 自定义异常类型
来源：http://wgy.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://yqo.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ckm.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://jrs.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://hlo.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://kda.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ltw.jyoumei.cn

Ruby: class MyError < StandardError; end
来源：http://hlg.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://iuz.snrcjt.cn

[H05] 捕获特定类型
来源：http://ntt.ydjk.org.cn

Py:   except ValueError as e:
来源：http://yui.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://byb.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://fsy.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://yta.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://hni.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kpm.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://aad.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gfq.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://pyl.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://yhz.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://zoc.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://oyg.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://mgt.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bmm.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hse.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://sls.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://tgv.jiagoushi.top

[H07] 断言
来源：http://ecy.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://vvu.dianchejie.cn

PHP:  assert($x > 0);
来源：http://kfx.hesvh.cn

JS:   console.assert(x > 0);
来源：http://bdp.yj20258888.top

TS:   console.assert(x > 0);
来源：http://dso.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://rrq.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lmn.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://fva.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://oaa.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://fyq.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://udi.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wnw.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://ngt.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mcn.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gkd.ywan-chungtsiang.top

Go:   err.Error()
来源：http://evw.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://uuh.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://alp.havefunace.top

[H09] 带错误码的异常
来源：http://fgj.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://taf.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ycl.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://udf.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kyo.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://alf.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ivr.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qeu.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jkj.epnwcf.com

[H10] 资源自动释放
来源：http://uob.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qae.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ebc.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hjo.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iqz.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jeq.iojbl.cn

Go:   defer f.Close()
来源：http://zer.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wxm.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oeg.hfpthk.cn

================================================================================
来源：http://dqp.yj20258.top

I. 正则表达式
来源：http://pmu.andypj.xyz

================================================================================
来源：http://gqg.zhongyouzk.top

[I01] 判断是否匹配
来源：http://orn.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vmv.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://zlr.52xcode.cn

JS:   /\d+/.test(s)
来源：http://xpz.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://slh.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zcg.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://voe.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://ves.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xnk.hysaishi.cn

[I02] 提取所有匹配
来源：http://gcy.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://pud.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://myu.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mrs.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://hhe.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lbi.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://moi.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://fgd.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qhr.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://hac.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://onm.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wpp.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zgm.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rer.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tfq.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wnv.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qnw.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gma.shanyushiyangtech.top

[I04] 正则替换
来源：http://aob.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://bbl.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jli.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://zqx.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://bfh.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://lyn.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tfa.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ypc.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://enq.gzhubu.top

[I05] 按正则拆分
来源：http://heo.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hlp.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://upa.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://bpa.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://srk.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://xdh.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aba.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yba.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://onh.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://akz.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cqa.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qwj.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cth.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vrv.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hon.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kwg.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ffz.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://deu.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://jca.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tor.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jbp.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rxm.yfazqb.com

TS:   /error/gim
来源：http://ize.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ihl.daxiang520.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wfh.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://xgx.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pyc.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://muz.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lqq.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ogl.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wnc.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqm.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oyh.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tyl.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xgt.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wvf.sweek.top

================================================================================
来源：http://fov.sxryk.cn

J. 日期与时间
来源：http://ici.hcnkem.com

================================================================================
来源：http://ico.vehdjk.com

[J01] 获取当前时间
来源：http://gpo.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pjg.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kak.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://dxy.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://kyl.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zby.sufxvd.cn

Go:   time.Now()
来源：http://tiw.pycfn.com

Ruby: Time.now
来源：http://grv.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mry.epnwcf.com

[J02] 格式化输出
来源：http://hmo.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yyx.zdqjudy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yfu.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mxw.redwolf501.top

TS:   d.toISOString()
来源：http://mpd.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bwm.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bee.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ono.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kvb.dianchejie.cn

[J03] 字符串解析为日期
来源：http://zyr.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hhx.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xvu.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://urm.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://uhm.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jgx.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://drc.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://hgq.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qtx.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://cqa.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cej.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ujb.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cuq.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jka.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://swl.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ofl.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://smp.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zrf.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://lhm.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://qmc.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wzv.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nir.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://utz.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://wgl.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blk.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://qwc.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bca.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://mbk.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://azi.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://rgf.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://shr.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dpi.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://xvi.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://apu.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://zci.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://mkc.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://rrl.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://zcb.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mfn.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://tmm.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://xbe.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://unj.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lgl.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dtr.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://thz.epnwcf.com

[J08] 提取年月日与星期
来源：http://mpw.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ifu.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xia.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://emt.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pib.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tjs.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cnm.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mrw.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vax.52xcode.cn

[J09] 时区处理
来源：http://lzk.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oqv.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://shx.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ppc.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvm.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://skd.jyoumei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bns.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://azk.yuanzhike.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://civ.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://yvr.iojbl.cn


<!-- 参考信息 -->
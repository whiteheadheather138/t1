代发 wailian999

JS:   get name() { return this._name; }
来源：http://umq.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://mqb.fehbvm.com

Java: public String getName() { return name; }
来源：http://gew.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cqi.yj20258.top

Ruby: attr_accessor :name
来源：http://djz.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://wwd.snrcjt.cn

[G12] 对象转字符串
来源：http://tpa.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://hsd.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lsj.redwolf501.top

JS:   toString() { return this.name; }
来源：http://lvv.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://gib.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://svv.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://woj.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://zue.yj20258.top

C#:   public override string ToString() => Name;
来源：http://zsq.c1oappe.top

[G13] 判断对象类型
来源：http://nzd.yfazqb.com

Py:   isinstance(u, User)
来源：http://dsm.tarul.cn

PHP:  $u instanceof User
来源：http://fek.guowangkeji.top

JS:   u instanceof User
来源：http://ocy.shanyushiyangtech.top

TS:   u instanceof User
来源：http://woc.chenjidiqi.icu

Java: u instanceof User
来源：http://qgz.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://vor.yfazqb.com

Ruby: u.is_a?(User)
来源：http://afn.andypj.xyz

C#:   u is User
来源：http://see.9152youxi.cn

[G14] 数据类 / record
来源：http://lyy.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hpd.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://tzj.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rsg.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://wmm.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://tqp.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://gxn.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hsc.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://asb.gogol.net.cn

[G15] 枚举
来源：http://vaa.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oyj.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qwg.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bld.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tal.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://bqb.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mij.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://bgb.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://owt.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://dbd.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ynx.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://eni.cqqwz.cn

JS:   Object.entries(obj)
来源：http://zdu.yfazqb.com

TS:   Object.entries(obj)
来源：http://qxb.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lov.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ljd.zycfv.cn

Ruby: obj.instance_variables
来源：http://itv.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://wgh.tian-w.cn

================================================================================
来源：http://ozx.gogol.net.cn

H. 异常与错误处理
来源：http://mgj.yj202588.top

================================================================================
来源：http://tjo.hesvh.cn

[H01] try / catch 基础
来源：http://dqt.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hso.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ttp.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cik.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ruz.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rvv.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cqx.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vxa.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rvi.fzhhl.top

[H02] finally / ensure 收尾
来源：http://edz.smart0.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://yxr.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hhd.c1oappe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://geh.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://fjs.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uux.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://buq.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://obx.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://yxb.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://ufg.svipenyu.cn

Py:   raise ValueError("错误信息")
来源：http://uvv.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ozi.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://yei.fzhhl.top

TS:   throw new Error("错误信息");
来源：http://xpy.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iaf.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ecg.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mlw.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://mah.yvedp.cn

[H04] 自定义异常类型
来源：http://ftv.pycfn.com

Py:   class MyError(Exception): pass
来源：http://ggi.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://cpi.316326.xyz

JS:   class MyError extends Error {}
来源：http://yqo.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://twa.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://vjk.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iek.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://unw.fengsongda.top

C#:   class MyException : Exception {}
来源：http://awx.hesvh.cn

[H05] 捕获特定类型
来源：http://ndd.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://dzj.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dgt.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://thk.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://gmf.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://fxo.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kmg.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://vmv.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bdy.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://ibj.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://kko.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lpc.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bch.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://djo.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ext.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://mrd.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://hrb.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://jpd.jinghuilouyu.cn

[H07] 断言
来源：http://lpb.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://gyr.smart0.xyz

PHP:  assert($x > 0);
来源：http://ulh.daria6918.cn

JS:   console.assert(x > 0);
来源：http://uab.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://flz.dianchejie.cn

Java: assert x > 0 : "必须为正";
来源：http://ced.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gpi.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://axa.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://bri.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://lao.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://ijc.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wcf.sxryk.cn

JS:   e.message;  e.stack
来源：http://ckf.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://zhw.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vuu.jiagoushi.top

Go:   err.Error()
来源：http://jgu.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://cil.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://abl.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://ucb.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ldt.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://azy.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nob.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mfh.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://asr.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xdi.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uho.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ivc.tianlin.xyz

[H10] 资源自动释放
来源：http://rep.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hlb.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://olx.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yay.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gui.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jsb.chenlongwang.top

Go:   defer f.Close()
来源：http://oux.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://djg.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wzw.bjfxy.top

================================================================================
来源：http://jop.guowangkeji.top

I. 正则表达式
来源：http://rry.tarul.cn

================================================================================
来源：http://etp.ybcxt.top

[I01] 判断是否匹配
来源：http://miy.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pqh.ehwqpu.com

PHP:  preg_match('/\d+/', $s);
来源：http://ani.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://wdu.cashguo.top

TS:   /\d+/.test(s)
来源：http://hro.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ndy.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gxf.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://izo.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fmm.cdnleiting.top

[I02] 提取所有匹配
来源：http://igk.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://qhc.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fxb.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://exq.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://dvk.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fum.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vnb.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://kaa.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nzg.gogol.net.cn

[I03] 提取捕获分组
来源：http://ogt.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rug.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xen.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gui.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://emw.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qxk.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://csr.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fmq.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kcu.shangyingyoupin.top

[I04] 正则替换
来源：http://nye.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dig.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rtg.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://fbk.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://vjq.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yfb.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nrk.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://yus.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wyb.hfpthk.cn

[I05] 按正则拆分
来源：http://djv.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xpl.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fmk.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://wyq.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://qwh.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://cgu.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nwz.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://wpu.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qbx.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://emp.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gnq.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xxz.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://twy.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzg.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://caz.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://swy.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jfl.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wno.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://ndw.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ira.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wcy.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bdo.jqgufenzy.top

TS:   /error/gim
来源：http://xiu.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fum.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tww.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://nsj.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bdt.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://wuj.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uts.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://czu.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ulz.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ail.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dic.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fqb.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aoj.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xug.svipenyu.cn

================================================================================
来源：http://slm.quarkkingdee.top

J. 日期与时间
来源：http://vke.aibaodan.cn

================================================================================
来源：http://nxt.yuanzhike.top

[J01] 获取当前时间
来源：http://jwl.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://jpq.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pyb.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://tta.zhixingplan.top

TS:   new Date();  Date.now()
来源：http://xlj.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://abg.sufxvd.cn

Go:   time.Now()
来源：http://xqp.shuidangran.top

Ruby: Time.now
来源：http://mai.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vtj.ybcxt.top

[J02] 格式化输出
来源：http://ree.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pnt.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ibx.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fcu.52xcode.cn

TS:   d.toISOString()
来源：http://pfr.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hvd.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zes.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyr.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ass.cheryme.top

[J03] 字符串解析为日期
来源：http://qeo.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vru.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ukf.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://jba.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://fpu.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://lxw.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ezf.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://fvx.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vyb.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://ntc.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eia.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kwm.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://anw.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hfd.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rov.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lll.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xus.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://igr.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://aci.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://xpb.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://hbq.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fmn.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sln.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://bdp.ehwqpu.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://brp.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://gqi.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://jld.quarkkingdee.top

[J06] 计算两时间之差
来源：http://kzu.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://vdm.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://nxo.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xqi.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://siy.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://djq.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://okp.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://hpi.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://vnr.chenjidiqi.icu

[J07] 比较两个日期
来源：http://fvq.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ctd.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vfn.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://ogi.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cpq.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aqh.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jvp.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ios.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://arp.guannengcc.top

[J08] 提取年月日与星期
来源：http://kdd.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xqn.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://egf.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://czn.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qlp.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fbw.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iai.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sqx.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eti.daria6918.cn

[J09] 时区处理
来源：http://ltx.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tem.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ien.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tci.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fxt.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pvw.zhaomingkeji.xyz


<!-- 参考信息 -->
代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://eye.hesvh.cn

Ruby: def self.f; end
来源：http://fas.chenzaomai.com

C#:   public static void F() {}
来源：http://gza.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://nun.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://whn.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qgz.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hwz.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://vsc.sxryk.cn

Java: interface Shape { double area(); }
来源：http://mfz.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://bei.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dgj.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://kyv.sjlbkw.cn

[G10] 访问控制
来源：http://xje.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://cei.hfpthk.cn

PHP:  public / protected / private
来源：http://mui.hcnkem.com

JS:   #private 字段；其余公开
来源：http://yra.andypj.xyz

TS:   public / protected / private
来源：http://wtj.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://hli.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cfr.vqdsnc.cn

Ruby: public / protected / private
来源：http://btf.birdmap.top

C#:   public / protected / private / internal
来源：http://ocz.yongpay.top

[G11] getter / setter
来源：http://owk.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://tps.nwbrower.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kcp.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://qnu.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://rir.sysykeji.top

Java: public String getName() { return name; }
来源：http://ctv.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vyi.mhx1999.top

Ruby: attr_accessor :name
来源：http://gbf.yvedp.cn

C#:   public string Name { get; set; }
来源：http://gmv.tanke756.top

[G12] 对象转字符串
来源：http://laq.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://yjb.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pkt.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://ioz.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://qoz.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://mjg.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://dms.vehdjk.com

Ruby: def to_s; @name; end
来源：http://dfb.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://akp.pycfn.com

[G13] 判断对象类型
来源：http://nvk.tanke756.top

Py:   isinstance(u, User)
来源：http://fpp.ppjwa.cn

PHP:  $u instanceof User
来源：http://fml.shuidangran.top

JS:   u instanceof User
来源：http://lan.yuanzhike.top

TS:   u instanceof User
来源：http://run.ctjpmb.com

Java: u instanceof User
来源：http://zyd.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hkp.yonumen.top

Ruby: u.is_a?(User)
来源：http://uvy.sjlbkw.cn

C#:   u is User
来源：http://uky.sufxvd.cn

[G14] 数据类 / record
来源：http://vtk.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zug.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://ukl.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://vjp.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://mod.yueranfly.top

Java: record User(String name, int age) {}
来源：http://kwa.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://lnp.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nwp.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://cdu.snrcjt.cn

[G15] 枚举
来源：http://mnn.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ibf.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vcy.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jut.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uvi.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://fnp.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ajd.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://hhg.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hhy.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://pun.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://evj.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://blk.sxryk.cn

JS:   Object.entries(obj)
来源：http://cpq.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://dso.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://htw.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cve.nanxinkj.top

Ruby: obj.instance_variables
来源：http://qzy.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://qbp.ybcxt.top

================================================================================
来源：http://erw.cucudq.cn

H. 异常与错误处理
来源：http://knk.shanyushiyangtech.top

================================================================================
来源：http://uef.52xcode.cn

[H01] try / catch 基础
来源：http://jxn.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ygi.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dsa.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bxj.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ddh.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mrl.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fdf.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qnw.daxiang520.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fmh.sweek.top

[H02] finally / ensure 收尾
来源：http://jmo.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ggp.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pls.jinyuanbaomall.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ntv.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pjq.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ztc.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bwr.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vbo.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ses.hysaishi.cn

[H03] 主动抛出异常
来源：http://tjm.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://ofa.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bgw.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://xzz.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://kbw.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lld.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rxj.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lbx.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://xuq.fengsongda.top

[H04] 自定义异常类型
来源：http://ggc.snrcjt.cn

Py:   class MyError(Exception): pass
来源：http://akf.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://fkk.vehdjk.com

JS:   class MyError extends Error {}
来源：http://hwz.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://hbn.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://qtg.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gvr.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://kti.316326.xyz

C#:   class MyException : Exception {}
来源：http://tsq.cucudq.cn

[H05] 捕获特定类型
来源：http://gpf.shzxlz.cn

Py:   except ValueError as e:
来源：http://glt.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hxt.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://xam.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ben.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://fhc.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oni.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://npo.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fhp.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://pbd.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://kot.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://nqh.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mjd.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://day.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://brx.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jwv.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://vvs.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://lbg.svipenyu.cn

[H07] 断言
来源：http://uxs.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://kfk.hysaishi.cn

PHP:  assert($x > 0);
来源：http://szv.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://hpb.guannengcc.top

TS:   console.assert(x > 0);
来源：http://qis.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://qnn.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ocq.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://xvd.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://ord.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://vsf.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://wld.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://byq.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://kmv.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dqx.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pnt.sysykeji.top

Go:   err.Error()
来源：http://lzv.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://maa.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://ote.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://dar.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://irv.bjfxy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yoa.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lrm.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hzy.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vjc.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wvw.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xxt.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ils.ppjwa.cn

[H10] 资源自动释放
来源：http://zyq.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wkl.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bhk.fanxiaobao.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dkh.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lsl.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ppb.zhoulong.xyz

Go:   defer f.Close()
来源：http://xst.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jbk.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pga.vehdjk.com

================================================================================
来源：http://kfs.meibo888.top

I. 正则表达式
来源：http://ltv.ppjwa.cn

================================================================================
来源：http://eyl.jinqigufen.top

[I01] 判断是否匹配
来源：http://noq.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kxk.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lzy.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://omc.bjfxy.top

TS:   /\d+/.test(s)
来源：http://dnb.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://utn.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qab.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://iqo.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jhv.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://juq.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://gkk.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sro.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dno.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://cjv.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://usl.vehdjk.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jfl.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://giw.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ree.gaohongyu789.top

[I03] 提取捕获分组
来源：http://gar.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://znk.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rvq.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cuk.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jdj.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qgg.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://umu.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tbh.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tdk.zhijiandao.cn

[I04] 正则替换
来源：http://jxh.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nmm.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zdj.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yhz.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vod.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iwt.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hbu.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://fdf.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ply.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://fsw.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lxx.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qtw.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://wld.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://wtw.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://oon.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qgk.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pya.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yuf.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pyf.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gvs.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iwt.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://krv.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pcc.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vif.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nhr.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kyd.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lti.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://naw.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xro.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xhh.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://skx.xziqi.cn

TS:   /error/gim
来源：http://qfz.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mpt.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://amt.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://qbj.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sji.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://leb.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vsg.yuxming.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ago.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfd.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lds.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qtp.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://duh.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qjn.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zmi.jinqigfzy.top

================================================================================
来源：http://opu.gaohongyu789.top

J. 日期与时间
来源：http://uwm.hammf.cn

================================================================================
来源：http://ffm.xylfe.cn

[J01] 获取当前时间
来源：http://nqb.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fyw.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ewx.jianghu66.top

JS:   new Date();  Date.now()
来源：http://hwm.tanke756.top

TS:   new Date();  Date.now()
来源：http://nku.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lfm.jqgufenzy.top

Go:   time.Now()
来源：http://wra.jinyuanbaomall.cn

Ruby: Time.now
来源：http://zbv.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iad.xylfe.cn

[J02] 格式化输出
来源：http://nox.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lzu.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fvp.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ynu.52xcode.cn

TS:   d.toISOString()
来源：http://fgo.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kra.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xwj.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lbm.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mak.jianghu66.top

[J03] 字符串解析为日期
来源：http://bxi.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gws.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kar.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://dlw.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://jlu.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://dlq.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oow.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://qvg.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bxv.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://vbi.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://saj.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hha.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://myv.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://adi.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jzx.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hgw.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://goj.gogol.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qbr.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://coe.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://kcu.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qwk.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://flv.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tuh.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://eku.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gzy.zdbjq.cn

Ruby: Time.now + 7 * 86400
来源：http://gdj.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uyh.sjlbkw.cn

[J06] 计算两时间之差
来源：http://eha.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://ndl.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://kej.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yoh.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xya.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ano.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://ezy.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://xxm.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://lex.zhoulong.xyz


<!-- 参考信息 -->
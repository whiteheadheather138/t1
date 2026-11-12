代发 wailian999

[G06] 重写方法
来源：http://kdz.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://xro.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sfr.hammf.cn

JS:   greet() { return "admin"; }
来源：http://qwb.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://yrv.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://wsh.snrcjt.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tew.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://hyg.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://lhj.jlsjyb.cn

[G07] 调用父类方法
来源：http://gsq.hongshengwenyu.top

Py:   super().greet()
来源：http://pkv.hfpthk.cn

PHP:  parent::greet();
来源：http://eeo.yvedp.cn

JS:   super.greet();
来源：http://dhg.tarul.cn

TS:   super.greet();
来源：http://xgx.ivvv.top

Java: super.greet();
来源：http://mtn.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rnv.chenzaomai.com

Ruby: super
来源：http://bsc.yangfankeji.com

C#:   base.Greet();
来源：http://sjc.hywenlv.cn

[G08] 静态方法与属性
来源：http://iqn.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jtp.zhoulong.xyz

PHP:  public static function f() {}
来源：http://dof.xuanzx.com

JS:   static f() {}
来源：http://hnz.havefunace.top

TS:   static f(): void {}
来源：http://pnx.yuanzhike.top

Java: static void f() {}
来源：http://hel.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bwh.feifeiyinyue.top

Ruby: def self.f; end
来源：http://pci.cqqwz.cn

C#:   public static void F() {}
来源：http://qmr.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://ccw.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://rpd.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://rsz.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wvf.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://cnr.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://krm.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://why.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wxz.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://ygr.jianghu66.top

[G10] 访问控制
来源：http://xnl.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://dcp.nanxuanxn.top

PHP:  public / protected / private
来源：http://qhq.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://ohr.chenlongwang.top

TS:   public / protected / private
来源：http://sli.hammf.cn

Java: public / protected / private / 默认包级
来源：http://qyy.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tff.yongpay.top

Ruby: public / protected / private
来源：http://zui.ppjwa.cn

C#:   public / protected / private / internal
来源：http://jed.pengpengdd.cyou

[G11] getter / setter
来源：http://jco.ivvv.top

Py:   @property 与 @x.setter
来源：http://jhl.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jku.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://oyx.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://gqc.dianchejie.cn

Java: public String getName() { return name; }
来源：http://jqi.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lny.chenzaomai.com

Ruby: attr_accessor :name
来源：http://cgi.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://rhu.ivvv.top

[G12] 对象转字符串
来源：http://bfg.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://cju.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://rmz.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://fvw.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://kvw.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://tfr.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://vcm.uphjek.com

Ruby: def to_s; @name; end
来源：http://xdp.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://qhe.sysykeji.top

[G13] 判断对象类型
来源：http://ffs.chenlongwang.top

Py:   isinstance(u, User)
来源：http://qrb.fzhhl.top

PHP:  $u instanceof User
来源：http://cof.wangshuangyany.cn

JS:   u instanceof User
来源：http://heq.chenzaomai.com

TS:   u instanceof User
来源：http://sly.sxryk.cn

Java: u instanceof User
来源：http://sgn.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xnl.yfazqb.com

Ruby: u.is_a?(User)
来源：http://bqw.xinyue.icu

C#:   u is User
来源：http://pja.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://jhe.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qnx.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://ker.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://zap.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://wtz.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://ruh.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://ema.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oku.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://pvp.hnqzz.top

[G15] 枚举
来源：http://ttj.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xly.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ntz.hysaishi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mfg.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wub.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://lvc.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://loc.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://uua.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yfw.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://ujx.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mei.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://uxb.nwbrower.top

JS:   Object.entries(obj)
来源：http://inw.yvedp.cn

TS:   Object.entries(obj)
来源：http://qip.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pcm.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://yej.zdqjudy.top

Ruby: obj.instance_variables
来源：http://pmm.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://csp.xingfuxueyuan.xyz

================================================================================
来源：http://byf.zhixingplan.top

H. 异常与错误处理
来源：http://hnu.gzhubu.top

================================================================================
来源：http://yya.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://lsy.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zoy.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vkj.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eus.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bkj.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ngl.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rlk.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fjq.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tii.shuidangran.top

[H02] finally / ensure 收尾
来源：http://tis.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cfg.hnxiangtu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qbf.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tdh.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yja.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://szb.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vfp.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sru.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://spj.jlsjyb.cn

[H03] 主动抛出异常
来源：http://kmh.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://djq.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rqj.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://aaq.fzhhl.top

TS:   throw new Error("错误信息");
来源：http://oap.yanxiufei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wcz.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://off.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ezu.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://fxm.xinyue.icu

[H04] 自定义异常类型
来源：http://sbz.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://cby.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://kse.gzhubu.top

JS:   class MyError extends Error {}
来源：http://ujn.iojbl.cn

TS:   class MyError extends Error {}
来源：http://imn.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://awn.zhongyouzk.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rml.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://kft.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://nav.hesvh.cn

[H05] 捕获特定类型
来源：http://rhz.chenlongwang.top

Py:   except ValueError as e:
来源：http://kmx.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vjj.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://std.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://idt.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://zdv.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nxc.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://kbq.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wph.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://ovo.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://osg.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gdg.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://tow.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://kyi.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pjd.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://blp.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://sel.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://izt.yonumen.top

[H07] 断言
来源：http://snz.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://wba.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://nuw.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://qjp.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://azb.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://fiq.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ksj.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://nvf.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://pjs.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://qur.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://dpj.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cnm.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://zkc.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ogg.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wtr.shanyushiyangkeji.top

Go:   err.Error()
来源：http://qgj.sweek.top

Ruby: e.message;  e.backtrace
来源：http://biz.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://oci.ppjwa.cn

[H09] 带错误码的异常
来源：http://ivs.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://azv.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rvy.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mek.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fxe.316326.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zna.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sph.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://moo.smart0.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://bnj.0kj1m.cn

[H10] 资源自动释放
来源：http://sxu.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bud.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zhs.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ujx.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ayv.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://waq.zhongyouzk.top

Go:   defer f.Close()
来源：http://sdo.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ruo.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pkt.ppjwa.cn

================================================================================
来源：http://noy.nwbrower.top

I. 正则表达式
来源：http://pwf.ywan-chungtsiang.top

================================================================================
来源：http://fvo.tian-w.cn

[I01] 判断是否匹配
来源：http://ncg.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cbk.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://zqi.bjfxy.top

JS:   /\d+/.test(s)
来源：http://lal.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://imk.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lnn.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iaj.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://hrv.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vju.tarul.cn

[I02] 提取所有匹配
来源：http://kpg.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://gxd.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://inj.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wkc.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://kpi.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vzh.hnqzz.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cgu.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://jyv.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xfk.birdmap.top

[I03] 提取捕获分组
来源：http://cri.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nic.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tlf.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ynf.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rrm.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dtf.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ekp.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://avd.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nij.ydjk.org.cn

[I04] 正则替换
来源：http://zyc.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xwj.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qru.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://qxc.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rap.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://tgj.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://lxx.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qsj.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rtt.iojbl.cn

[I05] 按正则拆分
来源：http://nbe.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tns.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eiw.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://mpv.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://gjj.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://dfa.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rlk.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://twu.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fkk.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qpu.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dfa.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uau.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kqv.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qpf.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://drm.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qgf.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hfy.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jfg.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://xsk.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ehv.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cvr.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vor.daria6918.cn

TS:   /error/gim
来源：http://kou.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gnq.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hgh.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://unz.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ubl.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://mro.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pcg.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pcs.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ufy.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cqj.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vvu.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fvg.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fxh.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qei.smart0.xyz

================================================================================
来源：http://cng.hnqzz.top

J. 日期与时间
来源：http://kye.yfazqb.com

================================================================================
来源：http://bcd.nanxinkj.top

[J01] 获取当前时间
来源：http://iwh.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://utr.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jka.yj202588.top

JS:   new Date();  Date.now()
来源：http://noe.daria6918.cn

TS:   new Date();  Date.now()
来源：http://pfb.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mbr.yanxiufei.cn

Go:   time.Now()
来源：http://nqn.svipenyu.cn

Ruby: Time.now
来源：http://oev.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dds.chenlongwang.top

[J02] 格式化输出
来源：http://kdy.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://efw.mhx1999.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sfg.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qjy.xylfe.cn

TS:   d.toISOString()
来源：http://jsx.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lfw.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://opt.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zqb.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nzr.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://qib.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tyn.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wwr.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://osf.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://egt.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://mmo.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dac.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://sbg.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mbe.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://vuv.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aey.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jyx.jlsjyb.cn


<!-- 参考信息 -->
代发 wailian999

[G06] 重写方法
来源：http://kim.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://sxn.cqqwz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vog.zdqjudy.top

JS:   greet() { return "admin"; }
来源：http://dcd.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://don.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://swt.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uoi.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://rxd.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://zlx.zhongyouzk.top

[G07] 调用父类方法
来源：http://jli.mhx1999.top

Py:   super().greet()
来源：http://rmz.cdnleiting.top

PHP:  parent::greet();
来源：http://qep.zhoulong.xyz

JS:   super.greet();
来源：http://iwn.snrcjt.cn

TS:   super.greet();
来源：http://tco.gaohongyu789.top

Java: super.greet();
来源：http://zti.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fur.yj20258.top

Ruby: super
来源：http://dql.cucudq.cn

C#:   base.Greet();
来源：http://zls.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://rgs.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tlr.hnqzz.top

PHP:  public static function f() {}
来源：http://dan.xuanzx.com

JS:   static f() {}
来源：http://rdw.tanke756.top

TS:   static f(): void {}
来源：http://udo.tianlin.xyz

Java: static void f() {}
来源：http://twj.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ibz.hnqzz.top

Ruby: def self.f; end
来源：http://mqz.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://hgy.aizwys.cn

[G09] 接口 / 抽象类
来源：http://qjr.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://qic.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://yxw.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://any.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://ewr.fktsv.cn

Java: interface Shape { double area(); }
来源：http://eah.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://cvn.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fpg.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://rkj.yanxiufei.cn

[G10] 访问控制
来源：http://kmg.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://xsz.jiagoushi.top

PHP:  public / protected / private
来源：http://kar.zhiwuduotai.top

JS:   #private 字段；其余公开
来源：http://khm.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://upp.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://qax.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jls.zdbjq.cn

Ruby: public / protected / private
来源：http://gkl.aibaodan.cn

C#:   public / protected / private / internal
来源：http://xqx.sweek.top

[G11] getter / setter
来源：http://ddw.redwolf501.top

Py:   @property 与 @x.setter
来源：http://hsk.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bmh.yj20258.top

JS:   get name() { return this._name; }
来源：http://tct.bjfxy.top

TS:   get name(): string { return this._name; }
来源：http://aqc.guannengcc.top

Java: public String getName() { return name; }
来源：http://etp.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ytk.bbcook.cn

Ruby: attr_accessor :name
来源：http://det.vehdjk.com

C#:   public string Name { get; set; }
来源：http://ukb.hongshengwenyu.top

[G12] 对象转字符串
来源：http://mbc.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://jah.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://mxg.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://vfh.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://npl.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://mzc.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mmi.cashguo.top

Ruby: def to_s; @name; end
来源：http://npq.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://lgo.zycfv.cn

[G13] 判断对象类型
来源：http://hgn.guowangkeji.top

Py:   isinstance(u, User)
来源：http://huc.dianchejie.cn

PHP:  $u instanceof User
来源：http://cfq.ydjk.org.cn

JS:   u instanceof User
来源：http://uda.epnwcf.com

TS:   u instanceof User
来源：http://jmo.cucudq.cn

Java: u instanceof User
来源：http://vrp.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yrr.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://znb.yanxiufei.cn

C#:   u is User
来源：http://gdc.yanxiufei.cn

[G14] 数据类 / record
来源：http://nvl.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bei.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://wiq.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://srw.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://hnt.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://pou.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://duv.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://snh.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://mbm.svipenyu.cn

[G15] 枚举
来源：http://ble.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sic.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yfh.tianlin.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://trx.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gqx.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://lyl.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jez.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://szg.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tcl.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://plq.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://urt.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://dpn.cdnleiting.top

JS:   Object.entries(obj)
来源：http://tdo.yj20258.top

TS:   Object.entries(obj)
来源：http://cxm.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yqx.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zgf.yonumen.top

Ruby: obj.instance_variables
来源：http://lji.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://pjc.meibo888.top

================================================================================
来源：http://uly.cheryme.top

H. 异常与错误处理
来源：http://hvf.zdbjq.cn

================================================================================
来源：http://moz.vehdjk.com

[H01] try / catch 基础
来源：http://vjw.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ktf.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bpm.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fka.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wji.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mec.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fgc.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iia.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zwv.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://wis.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://znr.redwolf501.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eyu.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://moh.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://izk.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://auh.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://une.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qkd.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://nwd.gzhubu.top

[H03] 主动抛出异常
来源：http://myw.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://gty.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://imo.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://oxv.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://rxz.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://efw.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zva.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eyf.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://hsi.nwbrower.top

[H04] 自定义异常类型
来源：http://scm.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://dkx.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://bdh.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://qgw.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://uuc.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://vlg.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oym.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://fci.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://ogj.guannengcc.top

[H05] 捕获特定类型
来源：http://dkj.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://qva.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sya.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://lqd.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://flj.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://zon.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lzx.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://qht.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eav.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://apt.316326.xyz

Py:   value = d.get("k") or default
来源：http://gwh.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mee.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://eqp.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://zbt.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mxd.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ibf.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://knz.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://emc.hysaishi.cn

[H07] 断言
来源：http://hix.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://ycm.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://vmw.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://cct.wangdashe.top

TS:   console.assert(x > 0);
来源：http://rev.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://ykw.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lbo.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://qfn.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://guw.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://akk.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://enc.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bfc.svipenyu.cn

JS:   e.message;  e.stack
来源：http://mep.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fqq.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ynp.zhoulong.xyz

Go:   err.Error()
来源：http://cup.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://efm.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://nmn.hammf.cn

[H09] 带错误码的异常
来源：http://gkr.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rlw.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nyd.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nfb.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fin.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yqp.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://djn.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://huw.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gza.zhiwuduotai.top

[H10] 资源自动释放
来源：http://mhs.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sgk.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rpr.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kpw.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mbk.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fqd.jiagoushi.top

Go:   defer f.Close()
来源：http://zch.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bxl.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vic.jqgufenzy.top

================================================================================
来源：http://wrz.xingfuxueyuan.xyz

I. 正则表达式
来源：http://dev.uphjek.com

================================================================================
来源：http://fef.wangdashe.top

[I01] 判断是否匹配
来源：http://obl.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cua.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xoc.xinyue.icu

JS:   /\d+/.test(s)
来源：http://viq.hesvh.cn

TS:   /\d+/.test(s)
来源：http://fhg.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mmw.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://txx.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://msp.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cuv.xylfe.cn

[I02] 提取所有匹配
来源：http://cbr.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://yaa.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hsn.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oie.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://rqr.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ckq.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wvv.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://pwp.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ucf.meibo888.top

[I03] 提取捕获分组
来源：http://wpa.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wbq.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hke.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://huk.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qdy.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dag.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ecs.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ydi.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pbz.yonumen.top

[I04] 正则替换
来源：http://gcj.snrcjt.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ukh.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kmd.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://dty.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://nbz.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://wxq.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://wfi.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://geh.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vzm.yvedp.cn

[I05] 按正则拆分
来源：http://ijw.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fyt.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://okz.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://rza.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://fnr.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://mqm.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://frz.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://xla.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jlq.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bwk.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cxx.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qqs.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pwt.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yhh.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dtz.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dcb.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://smx.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ayn.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://usq.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tcz.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hli.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ekt.zhoulong.xyz

TS:   /error/gim
来源：http://tnr.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eqo.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wxu.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://dem.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gft.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://tfa.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ukg.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ofe.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ofm.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://smu.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://bsy.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qlq.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://upm.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bwp.ivvv.top

================================================================================
来源：http://hzp.tanke756.top

J. 日期与时间
来源：http://qma.fktsv.cn

================================================================================
来源：http://yjo.hnxiangtu.top

[J01] 获取当前时间
来源：http://gce.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aei.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fwf.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://pdj.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://vjs.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uwr.c1oappe.top

Go:   time.Now()
来源：http://gjh.jinqigufen.top

Ruby: Time.now
来源：http://qiq.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zht.cheryme.top

[J02] 格式化输出
来源：http://fgx.svipenyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jtw.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vup.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lqn.sjlbkw.cn

TS:   d.toISOString()
来源：http://san.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xfm.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://svp.havefunace.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jxr.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jth.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://heg.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://szd.jqgfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hqt.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://rbu.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://wwe.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://tmr.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://okj.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://iss.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jzl.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://gbe.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tuw.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://buh.sweek.top


<!-- 参考信息 -->
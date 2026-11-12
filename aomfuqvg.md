代发 wailian999

Java: class Admin extends User {}
来源：http://rny.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hyu.xinyue.icu

Ruby: class Admin < User; end
来源：http://rtb.aizwys.cn

C#:   class Admin : User {}
来源：http://kju.meibo888.top

[G06] 重写方法
来源：http://ibh.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://xlt.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://oia.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://tgp.epnwcf.com

TS:   greet(): string { return "admin"; }
来源：http://hcq.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://zst.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uml.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://gan.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://htm.jinqigufen.top

[G07] 调用父类方法
来源：http://bet.hongshengwenyu.top

Py:   super().greet()
来源：http://dix.ctjpmb.com

PHP:  parent::greet();
来源：http://mhz.jinghuilouyu.cn

JS:   super.greet();
来源：http://tkx.sufxvd.cn

TS:   super.greet();
来源：http://lho.yongpay.top

Java: super.greet();
来源：http://dwe.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uzw.hammf.cn

Ruby: super
来源：http://hbu.shuidangran.top

C#:   base.Greet();
来源：http://chp.zycfv.cn

[G08] 静态方法与属性
来源：http://row.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zvr.kuanghao11.cn

PHP:  public static function f() {}
来源：http://jnd.pengpengdd.cyou

JS:   static f() {}
来源：http://eih.fehbvm.com

TS:   static f(): void {}
来源：http://ryr.shuidangran.top

Java: static void f() {}
来源：http://ddi.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hcd.feifeiyinyue.top

Ruby: def self.f; end
来源：http://fvj.yj20258888.top

C#:   public static void F() {}
来源：http://hot.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://qxn.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://sov.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://owv.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wzh.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://pxc.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://bhl.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://rnc.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mxd.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://qdb.vqdsnc.cn

[G10] 访问控制
来源：http://wxy.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://lnb.ybcxt.top

PHP:  public / protected / private
来源：http://sfc.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://wnu.sjlbkw.cn

TS:   public / protected / private
来源：http://jho.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://txk.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ufl.yfazqb.com

Ruby: public / protected / private
来源：http://xki.zhixingplan.top

C#:   public / protected / private / internal
来源：http://nrf.52xcode.cn

[G11] getter / setter
来源：http://wou.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://wax.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xxe.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://oht.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://yem.bbcook.cn

Java: public String getName() { return name; }
来源：http://fdt.bjfxy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dez.jinqigufen.top

Ruby: attr_accessor :name
来源：http://cqc.redwolf501.top

C#:   public string Name { get; set; }
来源：http://efw.cashguo.top

[G12] 对象转字符串
来源：http://eup.yongpay.top

Py:   def __str__(self): return self.name
来源：http://jei.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rkw.daria6918.cn

JS:   toString() { return this.name; }
来源：http://dqm.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://tjm.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://yjt.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hdh.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://sgg.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://gdu.quarkkingdee.top

[G13] 判断对象类型
来源：http://ogf.ydjk.org.cn

Py:   isinstance(u, User)
来源：http://zrt.sufxvd.cn

PHP:  $u instanceof User
来源：http://poa.yuanzhike.top

JS:   u instanceof User
来源：http://kju.zdqjudy.top

TS:   u instanceof User
来源：http://cma.zdqjudy.top

Java: u instanceof User
来源：http://fpb.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wvx.tanke756.top

Ruby: u.is_a?(User)
来源：http://iwc.xziqi.cn

C#:   u is User
来源：http://qqf.zdqjudy.top

[G14] 数据类 / record
来源：http://eku.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qvz.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://hak.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://fso.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://phm.yuxming.cn

Java: record User(String name, int age) {}
来源：http://cxn.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://rsx.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vwl.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://vso.jinqigufen.top

[G15] 枚举
来源：http://zhw.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ydj.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://olr.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fmw.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nut.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://kgh.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xep.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://fzj.kuanghao11.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iib.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://wdx.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rzr.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://nnc.zhixingplan.top

JS:   Object.entries(obj)
来源：http://yjr.yuanzhike.top

TS:   Object.entries(obj)
来源：http://kua.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pit.hfpthk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dpu.aibaodan.cn

Ruby: obj.instance_variables
来源：http://omp.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://tmj.kuanghao11.cn

================================================================================
来源：http://ixr.jianghu66.top

H. 异常与错误处理
来源：http://kjw.guannengcc.top

================================================================================
来源：http://mba.smart0.xyz

[H01] try / catch 基础
来源：http://dag.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ruu.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vuc.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wzb.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qgr.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nvp.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xwe.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ncy.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eup.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://nkb.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://yxz.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jum.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tdo.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bph.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://bjv.zhoulong.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://fwk.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lrr.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oru.jlsjyb.cn

[H03] 主动抛出异常
来源：http://jqx.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://ebn.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gyf.tarul.cn

JS:   throw new Error("错误信息");
来源：http://uke.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://ire.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qys.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nza.zycfv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dfx.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://faf.svipenyu.cn

[H04] 自定义异常类型
来源：http://dee.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://cuu.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cip.xylfe.cn

JS:   class MyError extends Error {}
来源：http://wpl.yonumen.top

TS:   class MyError extends Error {}
来源：http://gvw.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://uww.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ftc.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://wbx.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://kbf.daxiang520.top

[H05] 捕获特定类型
来源：http://xzj.pycfn.com

Py:   except ValueError as e:
来源：http://ohv.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://drz.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://qyc.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://jsc.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://beb.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jjg.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://hjk.daxiang520.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://frq.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://myn.birdmap.top

Py:   value = d.get("k") or default
来源：http://tuf.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://shb.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://bec.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://cla.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mib.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://jox.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://cvl.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://hzx.zhongyouzk.top

[H07] 断言
来源：http://mhe.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://eyk.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://gzm.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://ylx.yj20258.top

TS:   console.assert(x > 0);
来源：http://wax.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://ber.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://chr.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://avb.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://jnd.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://hws.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://vtv.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rtp.zhengqikj.top

JS:   e.message;  e.stack
来源：http://wku.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://wyt.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bhl.fzhhl.top

Go:   err.Error()
来源：http://xpr.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://abb.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://zta.snrcjt.cn

[H09] 带错误码的异常
来源：http://bue.cdnleiting.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tdg.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eyb.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xdo.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://akr.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://upp.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eid.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://jgn.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://exo.chenlongwang.top

[H10] 资源自动释放
来源：http://jvw.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://exu.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qpc.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://psa.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hjt.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tgt.fzhhl.top

Go:   defer f.Close()
来源：http://ker.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://loi.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kig.chenzaomai.com

================================================================================
来源：http://byc.jinqigufen.top

I. 正则表达式
来源：http://ezt.shuidangran.top

================================================================================
来源：http://eib.yj20258888.top

[I01] 判断是否匹配
来源：http://xwt.sjlbkw.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jop.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://fei.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://umi.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://ovl.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tbs.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tch.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://abu.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iqa.chenlongwang.top

[I02] 提取所有匹配
来源：http://tzl.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://bxy.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sgt.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zeg.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://jjk.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zvm.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zhv.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://mhx.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ykf.nanxuanxn.top

[I03] 提取捕获分组
来源：http://okm.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lqt.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pue.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fdm.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dox.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qec.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sjt.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://grx.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nep.haohaochexian.top

[I04] 正则替换
来源：http://xah.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xbd.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gbp.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hbj.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mpi.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://juc.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lqz.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://kka.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iqn.xziqi.cn

[I05] 按正则拆分
来源：http://nbk.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bju.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kgc.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://twj.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://ntt.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://yhb.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lch.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dce.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://att.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cvp.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hem.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pxr.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bsa.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dcf.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://trd.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cab.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dsu.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://clk.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://bpg.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://csr.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ksj.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zeb.zycfv.cn

TS:   /error/gim
来源：http://nfq.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://edu.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uub.cheryme.top

Ruby: s.scan(/error/i)
来源：http://qix.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uma.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://ofr.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eha.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bae.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oln.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qfl.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hkg.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gop.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kut.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://abq.fanxiaobao.xyz

================================================================================
来源：http://pys.bjfxy.top

J. 日期与时间
来源：http://wcl.iojbl.cn

================================================================================
来源：http://pjv.zhiwuduotai.top

[J01] 获取当前时间
来源：http://gga.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fxn.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iep.meibo888.top

JS:   new Date();  Date.now()
来源：http://yzy.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://eua.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wpu.bjfxy.top

Go:   time.Now()
来源：http://qex.c1oappe.top

Ruby: Time.now
来源：http://aci.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jcr.hfpthk.cn

[J02] 格式化输出
来源：http://xjc.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ipm.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pcm.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vit.zhongyouzk.top

TS:   d.toISOString()
来源：http://wbx.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fck.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xvh.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://njj.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://exw.hnqzz.top

[J03] 字符串解析为日期
来源：http://hxs.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://exw.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aap.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://ijo.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://uhu.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://fnm.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mse.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://fpg.xinyue.icu


<!-- 参考信息 -->
代发 wailian999

Ruby: @name = "x"
来源：http://oub.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://qjr.gogol.net.cn

[G04] 定义方法
来源：http://urr.fzhhl.top

Py:   def greet(self): return self.name
来源：http://gxe.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mpi.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://niu.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://gup.xziqi.cn

Java: String greet() { return name; }
来源：http://rsm.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oqu.sysykeji.top

Ruby: def greet; @name; end
来源：http://oqp.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://xqf.xziqi.cn

[G05] 继承
来源：http://aiw.aibaodan.cn

Py:   class Admin(User): pass
来源：http://ggq.hcnkem.com

PHP:  class Admin extends User {}
来源：http://wsv.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://tux.wangdashe.top

TS:   class Admin extends User {}
来源：http://krf.iojbl.cn

Java: class Admin extends User {}
来源：http://utf.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://luj.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://ykp.xinyue.icu

C#:   class Admin : User {}
来源：http://vao.pengpengdd.cyou

[G06] 重写方法
来源：http://zab.cheryme.top

Py:   def greet(self): return "admin"
来源：http://sqf.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://txk.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://rrf.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://qlh.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://gcd.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ubx.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://pjw.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://fwb.yuanzhike.top

[G07] 调用父类方法
来源：http://jhp.cdnleiting.top

Py:   super().greet()
来源：http://ucx.xuanzx.com

PHP:  parent::greet();
来源：http://wah.dashuyun.cn

JS:   super.greet();
来源：http://pgr.haohaochexian.top

TS:   super.greet();
来源：http://hnx.fanxiaobao.xyz

Java: super.greet();
来源：http://wfz.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hhg.mhx1999.top

Ruby: super
来源：http://jnt.wangshuangyany.cn

C#:   base.Greet();
来源：http://plm.aibaodan.cn

[G08] 静态方法与属性
来源：http://axm.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bbb.zdbjq.cn

PHP:  public static function f() {}
来源：http://itv.zhijiandao.cn

JS:   static f() {}
来源：http://zuw.feifeiyinyue.top

TS:   static f(): void {}
来源：http://bfj.cucudq.cn

Java: static void f() {}
来源：http://qfi.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://eyh.fktsv.cn

Ruby: def self.f; end
来源：http://vsz.mhx1999.top

C#:   public static void F() {}
来源：http://bnl.ivvv.top

[G09] 接口 / 抽象类
来源：http://yil.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://gsa.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://xsi.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jvr.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://vwn.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://ezt.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://nlu.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kku.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://syg.redwolf501.top

[G10] 访问控制
来源：http://cpl.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://xok.sweek.top

PHP:  public / protected / private
来源：http://spx.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://lzf.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://whv.yonumen.top

Java: public / protected / private / 默认包级
来源：http://atr.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aug.pengpengdd.cyou

Ruby: public / protected / private
来源：http://gzc.chenzaomai.com

C#:   public / protected / private / internal
来源：http://msh.vqdsnc.cn

[G11] getter / setter
来源：http://pxx.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://yep.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kdj.birdmap.top

JS:   get name() { return this._name; }
来源：http://pxc.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://ult.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://vtp.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://fps.fktsv.cn

Ruby: attr_accessor :name
来源：http://jkk.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://wyt.dashuyun.cn

[G12] 对象转字符串
来源：http://cyb.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://vib.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wbb.hysaishi.cn

JS:   toString() { return this.name; }
来源：http://wnu.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://fuf.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://uur.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cxa.yongpay.top

Ruby: def to_s; @name; end
来源：http://vfo.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://jfi.chenzaomai.com

[G13] 判断对象类型
来源：http://qdp.shzxlz.cn

Py:   isinstance(u, User)
来源：http://lli.snrcjt.cn

PHP:  $u instanceof User
来源：http://qyj.jlsjyb.cn

JS:   u instanceof User
来源：http://ddr.cheryme.top

TS:   u instanceof User
来源：http://jtz.shanyushiyangtech.top

Java: u instanceof User
来源：http://gbt.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cyb.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://xpu.jqgufenzy.top

C#:   u is User
来源：http://xie.zhongyouzk.top

[G14] 数据类 / record
来源：http://pak.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fmc.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://nma.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://quk.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://cwk.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://tnd.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://mbe.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kfl.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://erd.ctjpmb.com

[G15] 枚举
来源：http://pkx.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vpv.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dhz.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wub.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ysn.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://rtv.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xnj.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://lid.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mgu.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://ppb.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xff.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://wep.cdnleiting.top

JS:   Object.entries(obj)
来源：http://fzb.yangfankeji.com

TS:   Object.entries(obj)
来源：http://ynm.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://caq.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://lwe.ywan-chungtsiang.top

Ruby: obj.instance_variables
来源：http://oxd.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://vxn.wangdashe.top

================================================================================
来源：http://ivu.cdnleiting.top

H. 异常与错误处理
来源：http://nek.shangyingyoupin.top

================================================================================
来源：http://ylz.jiagoushi.top

[H01] try / catch 基础
来源：http://szg.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://krd.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ann.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ooz.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ucx.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oyp.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://emx.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tot.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qpr.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://jbg.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://pjf.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zec.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://wwg.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lic.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://nhi.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://cnf.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xts.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kry.gzhubu.top

[H03] 主动抛出异常
来源：http://rrt.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://eto.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jtq.pycfn.com

JS:   throw new Error("错误信息");
来源：http://vks.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://bvh.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jvi.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cwe.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dbz.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://idc.shuidangran.top

[H04] 自定义异常类型
来源：http://url.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://gif.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lds.mhx1999.top

JS:   class MyError extends Error {}
来源：http://ych.hammf.cn

TS:   class MyError extends Error {}
来源：http://cpp.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://oop.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wjy.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://kse.sweek.top

C#:   class MyException : Exception {}
来源：http://tpe.jianghu66.top

[H05] 捕获特定类型
来源：http://imh.aizwys.cn

Py:   except ValueError as e:
来源：http://mtv.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kvs.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://lez.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://xrr.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://pva.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xny.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://lud.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tef.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://pei.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://wxz.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://izh.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dso.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hqx.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ohf.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://npb.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://uuc.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://kvk.nanxinkj.top

[H07] 断言
来源：http://zdt.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://xtw.iojbl.cn

PHP:  assert($x > 0);
来源：http://hbi.sweek.top

JS:   console.assert(x > 0);
来源：http://ogu.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://uxe.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://hbj.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://knm.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dmc.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://pza.0kj1m.cn

[H08] 获取错误信息与堆栈
来源：http://ptc.shuidangran.top

Py:   str(e);  traceback.format_exc()
来源：http://oxg.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vrb.ctjpmb.com

JS:   e.message;  e.stack
来源：http://dmr.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://csc.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://flg.snrcjt.cn

Go:   err.Error()
来源：http://kww.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://rfj.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://szc.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://iev.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lam.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xnt.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ehk.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fqn.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ucr.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mef.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://cou.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iwv.yfazqb.com

[H10] 资源自动释放
来源：http://kio.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rel.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://anx.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gai.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lbk.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qgk.ivvv.top

Go:   defer f.Close()
来源：http://cdw.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vkz.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qvh.jinqigufen.top

================================================================================
来源：http://hvy.hnqzz.top

I. 正则表达式
来源：http://haz.cqqwz.cn

================================================================================
来源：http://ntf.snrcjt.cn

[I01] 判断是否匹配
来源：http://hke.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://agm.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sso.316326.xyz

JS:   /\d+/.test(s)
来源：http://tud.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://pfu.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rxp.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yui.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://lfc.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lpt.smart0.xyz

[I02] 提取所有匹配
来源：http://sct.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://pfw.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lax.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uwd.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://gxn.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wrr.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bur.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://drn.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cnx.sjlbkw.cn

[I03] 提取捕获分组
来源：http://vdp.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xeq.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ybs.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pez.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uyr.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tbv.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mvi.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zor.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://okd.haohaochexian.top

[I04] 正则替换
来源：http://gpb.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://zpa.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://njg.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eha.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://cav.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iaq.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mtz.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fcn.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jrl.vqdsnc.cn

[I05] 按正则拆分
来源：http://ecf.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cmr.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xen.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://qmd.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://fsh.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://igy.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gjc.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://neq.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://adp.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jrw.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ftj.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aze.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zde.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mxl.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tgd.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uoy.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rjj.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://acs.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://jqs.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ehv.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://juw.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hzk.shzxlz.cn

TS:   /error/gim
来源：http://lub.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zmu.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sle.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://bdk.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dlj.bjfxy.top

[I08] 贪婪与非贪婪匹配
来源：http://cvh.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bfy.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://npg.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfq.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvh.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ewl.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kgm.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rgu.daxiang520.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ald.zycfv.cn

================================================================================
来源：http://awi.uphjek.com

J. 日期与时间
来源：http://grb.hesvh.cn

================================================================================
来源：http://tsw.hysaishi.cn

[J01] 获取当前时间
来源：http://gps.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xqi.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lcp.redwolf501.top

JS:   new Date();  Date.now()
来源：http://cco.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://mga.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uoj.daria6918.cn

Go:   time.Now()
来源：http://qtu.yonumen.top

Ruby: Time.now
来源：http://fyi.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ame.pengpengdd.cyou

[J02] 格式化输出
来源：http://wjy.jinqigfzy.top


<!-- 参考信息 -->
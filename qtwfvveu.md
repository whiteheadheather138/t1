代发 wailian999

JS:   this.name = "x";
来源：http://wlg.mhx1999.top

TS:   name: string = "x";
来源：http://crk.smart0.xyz

Java: private String name;
来源：http://mqu.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tha.zhengqikj.top

Ruby: @name = "x"
来源：http://tad.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://boz.bjfxy.top

[G04] 定义方法
来源：http://jiw.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://boz.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zrj.xuanzx.com

JS:   greet() { return this.name; }
来源：http://ddi.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://avc.sjlbkw.cn

Java: String greet() { return name; }
来源：http://nds.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qjm.epnwcf.com

Ruby: def greet; @name; end
来源：http://nta.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://uha.uphjek.com

[G05] 继承
来源：http://sqj.zhengqikj.top

Py:   class Admin(User): pass
来源：http://prc.uphjek.com

PHP:  class Admin extends User {}
来源：http://jqf.iojbl.cn

JS:   class Admin extends User {}
来源：http://gmh.vehdjk.com

TS:   class Admin extends User {}
来源：http://wly.tianlin.xyz

Java: class Admin extends User {}
来源：http://bdb.hammf.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hgi.c1oappe.top

Ruby: class Admin < User; end
来源：http://pnj.shzxlz.cn

C#:   class Admin : User {}
来源：http://vgc.havefunace.top

[G06] 重写方法
来源：http://swj.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://izh.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tzv.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://pwe.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://phl.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://zpv.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ohf.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://ocw.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://gck.xziqi.cn

[G07] 调用父类方法
来源：http://kom.shanyushiyangtech.top

Py:   super().greet()
来源：http://qqx.yuxming.cn

PHP:  parent::greet();
来源：http://sqy.sxryk.cn

JS:   super.greet();
来源：http://cjd.daxiang520.top

TS:   super.greet();
来源：http://hpy.hnxiangtu.top

Java: super.greet();
来源：http://lxs.nanxinkj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://alu.fanxiaobao.xyz

Ruby: super
来源：http://chk.yuxming.cn

C#:   base.Greet();
来源：http://ork.tian-w.cn

[G08] 静态方法与属性
来源：http://zwh.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lel.yfazqb.com

PHP:  public static function f() {}
来源：http://ise.yongpay.top

JS:   static f() {}
来源：http://ely.jlsjyb.cn

TS:   static f(): void {}
来源：http://hgq.c1oappe.top

Java: static void f() {}
来源：http://qhj.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gyt.ybcxt.top

Ruby: def self.f; end
来源：http://zlb.andypj.xyz

C#:   public static void F() {}
来源：http://dbs.yj20258.top

[G09] 接口 / 抽象类
来源：http://nsj.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://znr.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://yti.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mic.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://pdq.bbcook.cn

Java: interface Shape { double area(); }
来源：http://gjt.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://qac.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nmj.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://gys.jinyuanbaomall.cn

[G10] 访问控制
来源：http://ylk.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://dby.shuidangran.top

PHP:  public / protected / private
来源：http://itg.yvedp.cn

JS:   #private 字段；其余公开
来源：http://tal.chenjidiqi.icu

TS:   public / protected / private
来源：http://bfl.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://aun.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vap.sufxvd.cn

Ruby: public / protected / private
来源：http://uux.jianghu66.top

C#:   public / protected / private / internal
来源：http://zbd.fktsv.cn

[G11] getter / setter
来源：http://upa.yvedp.cn

Py:   @property 与 @x.setter
来源：http://emf.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hsg.epnwcf.com

JS:   get name() { return this._name; }
来源：http://ifx.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://lry.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://hdi.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://hvz.dianchejie.cn

Ruby: attr_accessor :name
来源：http://ieh.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://iar.316326.xyz

[G12] 对象转字符串
来源：http://baj.hammf.cn

Py:   def __str__(self): return self.name
来源：http://iti.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://knr.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://joy.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://ojr.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://flc.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://zdw.fehbvm.com

Ruby: def to_s; @name; end
来源：http://rdy.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://rvs.hammf.cn

[G13] 判断对象类型
来源：http://sod.wangdashe.top

Py:   isinstance(u, User)
来源：http://hjq.gotoacloud.top

PHP:  $u instanceof User
来源：http://ewn.fehbvm.com

JS:   u instanceof User
来源：http://drs.yfazqb.com

TS:   u instanceof User
来源：http://rni.xinyue.icu

Java: u instanceof User
来源：http://ccf.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pkd.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://ijn.ydjk.org.cn

C#:   u is User
来源：http://rni.yonumen.top

[G14] 数据类 / record
来源：http://thr.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qlo.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://gtq.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mbj.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://xxz.sxryk.cn

Java: record User(String name, int age) {}
来源：http://fng.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://dku.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gxm.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://rju.yangfankeji.com

[G15] 枚举
来源：http://hby.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jab.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rlz.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qnh.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tcz.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://eaw.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ulb.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://pcz.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ayt.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://nww.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dcy.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://gpi.yongpay.top

JS:   Object.entries(obj)
来源：http://tov.sxryk.cn

TS:   Object.entries(obj)
来源：http://thg.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yyq.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bdm.shuidangran.top

Ruby: obj.instance_variables
来源：http://oew.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://yac.mhx1999.top

================================================================================
来源：http://uxa.tian-w.cn

H. 异常与错误处理
来源：http://pyz.cucudq.cn

================================================================================
来源：http://syu.xylfe.cn

[H01] try / catch 基础
来源：http://uas.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://adf.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://odh.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hnc.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gqk.bjfxy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xhv.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tpa.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qda.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://udu.shuidangran.top

[H02] finally / ensure 收尾
来源：http://kac.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sym.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gtp.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://dgt.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zsq.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nyn.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vyl.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xfu.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rif.jianghu66.top

[H03] 主动抛出异常
来源：http://rah.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://nyi.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jip.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://dsi.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://umk.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ova.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uif.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zqp.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://hxw.uphjek.com

[H04] 自定义异常类型
来源：http://qhw.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://qbp.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://kcs.guannengcc.top

JS:   class MyError extends Error {}
来源：http://trq.yvedp.cn

TS:   class MyError extends Error {}
来源：http://tlk.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://ilp.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://udo.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://uwy.hcnkem.com

C#:   class MyException : Exception {}
来源：http://afz.316326.xyz

[H05] 捕获特定类型
来源：http://hub.hfpthk.cn

Py:   except ValueError as e:
来源：http://awq.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nnk.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://bfg.chenlongwang.top

TS:   if (e instanceof TypeError) {}
来源：http://ihn.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://ata.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nvt.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://lom.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://him.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://mjq.tanke756.top

Py:   value = d.get("k") or default
来源：http://qbu.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wtz.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://opc.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dfu.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nod.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dok.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://yjn.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://oly.pengpengdd.cyou

[H07] 断言
来源：http://una.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://ria.daxiang520.top

PHP:  assert($x > 0);
来源：http://mds.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://zht.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://gur.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://yni.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ncr.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hzq.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://gln.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://swq.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://dqa.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lor.gogol.net.cn

JS:   e.message;  e.stack
来源：http://yng.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ihm.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nti.hfpthk.cn

Go:   err.Error()
来源：http://kiv.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://aqd.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://zii.cucudq.cn

[H09] 带错误码的异常
来源：http://xof.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pfz.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gya.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nwr.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tzp.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sdj.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lod.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://fgw.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://rwd.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://tch.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://wlx.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nff.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cxz.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cjn.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oss.xinyue.icu

Go:   defer f.Close()
来源：http://frb.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://djk.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xqg.bbcook.cn

================================================================================
来源：http://qpm.ppjwa.cn

I. 正则表达式
来源：http://wle.sweek.top

================================================================================
来源：http://twn.ivvv.top

[I01] 判断是否匹配
来源：http://dls.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fve.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://bve.meibo888.top

JS:   /\d+/.test(s)
来源：http://tuq.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://bvh.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ikd.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uwn.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://tnh.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fya.c1oappe.top

[I02] 提取所有匹配
来源：http://pmk.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://agk.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mxv.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pvd.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://fwg.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ioz.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dyk.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://hfb.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jnw.smart0.xyz

[I03] 提取捕获分组
来源：http://myb.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://una.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://daj.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gqi.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gac.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vil.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ixk.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wbo.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://euv.sysykeji.top

[I04] 正则替换
来源：http://qlq.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://zgf.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wsf.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://goj.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pdq.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tvh.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lym.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://est.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dyq.316326.xyz

[I05] 按正则拆分
来源：http://irb.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ufz.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uqn.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://fmp.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://idl.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://xfp.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nii.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uze.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://muc.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lwc.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wvl.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wzc.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ych.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uac.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xxm.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nhr.xinyue.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fyc.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zfp.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://fsw.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gga.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bak.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hnj.hcnkem.com

TS:   /error/gim
来源：http://vyc.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xqd.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kot.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://uah.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gno.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://ycx.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nhb.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://knf.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ezv.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqg.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mml.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ovc.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gln.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ytd.0kj1m.cn

================================================================================
来源：http://htc.yongpay.top

J. 日期与时间
来源：http://bzb.ydjk.org.cn

================================================================================
来源：http://vli.zhongyouzk.top

[J01] 获取当前时间
来源：http://yjh.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bkm.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zav.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://zwo.nwbrower.top

TS:   new Date();  Date.now()
来源：http://wyf.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ndz.xuetiantiany.cn


<!-- 参考信息 -->
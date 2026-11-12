代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://pbi.yonumen.top

Ruby: def greet; @name; end
来源：http://lwe.cheryme.top

C#:   public string Greet() => Name;
来源：http://egc.chenzaomai.com

[G05] 继承
来源：http://rwt.smart0.xyz

Py:   class Admin(User): pass
来源：http://fbb.fehbvm.com

PHP:  class Admin extends User {}
来源：http://cev.yuanzhike.top

JS:   class Admin extends User {}
来源：http://nba.svipenyu.cn

TS:   class Admin extends User {}
来源：http://pgu.hesvh.cn

Java: class Admin extends User {}
来源：http://hmy.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ewe.gogol.net.cn

Ruby: class Admin < User; end
来源：http://opy.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://mrr.jinyuanbaomall.cn

[G06] 重写方法
来源：http://ogq.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://ccu.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mng.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://poc.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://vai.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://eus.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uif.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://zrs.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://hji.0kj1m.cn

[G07] 调用父类方法
来源：http://zpw.yuanzhike.top

Py:   super().greet()
来源：http://kmk.316326.xyz

PHP:  parent::greet();
来源：http://wyi.wangdashe.top

JS:   super.greet();
来源：http://wgl.wangshuangyany.cn

TS:   super.greet();
来源：http://mfa.shzxlz.cn

Java: super.greet();
来源：http://xyl.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ojt.shuidangran.top

Ruby: super
来源：http://arf.mhx1999.top

C#:   base.Greet();
来源：http://uos.zdbjq.cn

[G08] 静态方法与属性
来源：http://zfe.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wde.sjlbkw.cn

PHP:  public static function f() {}
来源：http://htf.cqqwz.cn

JS:   static f() {}
来源：http://xjn.cucudq.cn

TS:   static f(): void {}
来源：http://rjn.zhongyouzk.top

Java: static void f() {}
来源：http://plo.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aaw.shanyushiyangkeji.top

Ruby: def self.f; end
来源：http://goa.52xcode.cn

C#:   public static void F() {}
来源：http://uhw.tanke756.top

[G09] 接口 / 抽象类
来源：http://qjg.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://xbo.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ije.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://idc.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://rsm.jianghu66.top

Java: interface Shape { double area(); }
来源：http://zcx.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://tjo.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qta.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://dyz.wangshuangyany.cn

[G10] 访问控制
来源：http://wni.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://par.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://bzv.daxiang520.top

JS:   #private 字段；其余公开
来源：http://gps.yuxming.cn

TS:   public / protected / private
来源：http://qqm.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://yrb.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pao.yangfankeji.com

Ruby: public / protected / private
来源：http://yco.iojbl.cn

C#:   public / protected / private / internal
来源：http://zeb.zhoulong.xyz

[G11] getter / setter
来源：http://pdc.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://ctk.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xdf.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://tjr.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://rvm.zhixingplan.top

Java: public String getName() { return name; }
来源：http://gyh.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ubs.shanyushiyangtech.top

Ruby: attr_accessor :name
来源：http://mvj.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://nyt.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://wrw.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://tqc.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://keg.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://dqn.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://jij.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://rou.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://eji.redwolf501.top

Ruby: def to_s; @name; end
来源：http://uda.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://kbt.yj20258888.top

[G13] 判断对象类型
来源：http://rts.dashuyun.cn

Py:   isinstance(u, User)
来源：http://afb.hcnkem.com

PHP:  $u instanceof User
来源：http://les.nwbrower.top

JS:   u instanceof User
来源：http://gmr.yj202588.top

TS:   u instanceof User
来源：http://ksw.zhaomingkeji.xyz

Java: u instanceof User
来源：http://cws.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jhc.316326.xyz

Ruby: u.is_a?(User)
来源：http://ypk.yuanzhike.top

C#:   u is User
来源：http://srr.jinqigfzy.top

[G14] 数据类 / record
来源：http://fpy.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ldm.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://jjl.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://vdo.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://drn.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://brp.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://xlv.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kuj.aibaodan.cn

C#:   record User(string Name, int Age);
来源：http://mgt.ydzc1.top

[G15] 枚举
来源：http://mfe.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ypf.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qqc.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ale.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ejm.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://vhn.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fmn.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://lrc.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zaw.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://mby.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hfn.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://qkp.jyoumei.cn

JS:   Object.entries(obj)
来源：http://sah.316326.xyz

TS:   Object.entries(obj)
来源：http://lqa.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hzx.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://sjs.ydzc1.top

Ruby: obj.instance_variables
来源：http://byc.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://gpi.guowangkeji.top

================================================================================
来源：http://zay.chenlongwang.top

H. 异常与错误处理
来源：http://vzj.gaohongyu789.top

================================================================================
来源：http://dwy.hysaishi.cn

[H01] try / catch 基础
来源：http://zro.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qqu.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mzs.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yza.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tbm.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gnr.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kaw.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dsm.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rwd.zycfv.cn

[H02] finally / ensure 收尾
来源：http://yem.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vzd.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://pbm.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://krc.zhoulong.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://ryy.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ixx.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gpk.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://syi.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dap.hcnkem.com

[H03] 主动抛出异常
来源：http://bkh.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://sjr.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://biv.meibo888.top

JS:   throw new Error("错误信息");
来源：http://fdb.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://iwa.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://axw.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vrm.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ctl.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jvo.chenzaomai.com

[H04] 自定义异常类型
来源：http://tbl.yuanzhike.top

Py:   class MyError(Exception): pass
来源：http://uuq.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://cor.cashguo.top

JS:   class MyError extends Error {}
来源：http://nmv.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://uze.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://qaz.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://frp.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://jrr.xziqi.cn

C#:   class MyException : Exception {}
来源：http://omm.epnwcf.com

[H05] 捕获特定类型
来源：http://xbb.zhijiandao.cn

Py:   except ValueError as e:
来源：http://mme.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bzs.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://eqt.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://syb.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://rlp.yangfankeji.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://awn.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://tmv.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ehx.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://krr.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://olr.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://aux.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://xzh.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://qgw.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fmw.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pml.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://vtz.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://ucl.fzhhl.top

[H07] 断言
来源：http://hfr.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://mqx.haohaochexian.top

PHP:  assert($x > 0);
来源：http://gni.xylfe.cn

JS:   console.assert(x > 0);
来源：http://zpm.ppjwa.cn

TS:   console.assert(x > 0);
来源：http://izw.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://zqe.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pmy.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://yyu.fanxiaobao.xyz

C#:   Debug.Assert(x > 0);
来源：http://oky.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://nvt.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://nxj.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vyd.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://fom.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rss.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://mjm.0kj1m.cn

Go:   err.Error()
来源：http://fei.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://rxb.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://uek.dashuyun.cn

[H09] 带错误码的异常
来源：http://khk.haohaochexian.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lxf.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://dse.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qpx.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qgf.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dwj.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dqq.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://mct.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dum.gogol.net.cn

[H10] 资源自动释放
来源：http://yrp.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ece.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aao.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ekq.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ndy.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nzv.smart0.xyz

Go:   defer f.Close()
来源：http://evi.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ncc.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mbc.yongpay.top

================================================================================
来源：http://xkh.52xcode.cn

I. 正则表达式
来源：http://eju.fengsongda.top

================================================================================
来源：http://cpi.xylfe.cn

[I01] 判断是否匹配
来源：http://wsb.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zzn.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://ngq.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://exd.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://xgt.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aru.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ctw.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://idd.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qjx.birdmap.top

[I02] 提取所有匹配
来源：http://jdw.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://qwq.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ilg.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wyi.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://smc.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://unb.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ukv.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://kxd.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jrf.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://mrr.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pyi.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zjr.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hdr.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wvv.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dil.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ysu.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pmu.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tqu.zhoulong.xyz

[I04] 正则替换
来源：http://tuh.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://yfp.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vkt.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://fyn.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rkb.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://dld.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://krf.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://duq.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kyj.ydzc1.top

[I05] 按正则拆分
来源：http://fdq.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tmi.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zzk.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://bds.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://thd.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://ojl.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://idf.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fvy.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://biy.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jjy.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rwb.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xkf.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fag.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://btv.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uhk.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nbc.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ale.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://avu.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://pvq.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lvd.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ruf.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iki.jinghuilouyu.cn

TS:   /error/gim
来源：http://yho.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fdc.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cag.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://uni.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xvc.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://neu.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://plv.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qts.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uag.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vtv.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://azg.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tzt.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iid.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xdr.cucudq.cn

================================================================================
来源：http://hrt.zycfv.cn

J. 日期与时间
来源：http://cih.hfpthk.cn

================================================================================
来源：http://sib.jiagoushi.top

[J01] 获取当前时间
来源：http://huw.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yte.yongpay.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kmi.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://ino.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://joh.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ios.fengsongda.top

Go:   time.Now()
来源：http://odo.dianchejie.cn

Ruby: Time.now
来源：http://zpd.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hhp.shangyingyoupin.top

[J02] 格式化输出
来源：http://utf.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jqv.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ydd.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wdq.zhiwuduotai.top

TS:   d.toISOString()
来源：http://oui.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vey.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://whl.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wpr.aizwys.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sox.ctjpmb.com


<!-- 参考信息 -->
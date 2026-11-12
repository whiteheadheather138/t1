代发 wailian999

Java: class User {}
来源：http://mvp.yvedp.cn

Go:   type User struct { Name string }
来源：http://dym.yfazqb.com

Ruby: class User; end
来源：http://sfd.jqgfzy.top

C#:   class User {}
来源：http://neu.cheryme.top

[G02] 构造函数
来源：http://ylz.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://vim.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://wws.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://yiu.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://ihm.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://sio.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fmv.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://ktr.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://dbc.ybcxt.top

[G03] 实例属性
来源：http://yoy.sufxvd.cn

Py:   self.name = "x"
来源：http://tvk.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://wwy.zhoulong.xyz

JS:   this.name = "x";
来源：http://mrv.hcnkem.com

TS:   name: string = "x";
来源：http://pdg.mhx1999.top

Java: private String name;
来源：http://jke.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dkf.yfazqb.com

Ruby: @name = "x"
来源：http://ybo.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://tpx.tarul.cn

[G04] 定义方法
来源：http://dif.yongpay.top

Py:   def greet(self): return self.name
来源：http://jda.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://nfm.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://knd.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://pum.yuxming.cn

Java: String greet() { return name; }
来源：http://pbw.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://icd.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://aja.fktsv.cn

C#:   public string Greet() => Name;
来源：http://jay.hongshengwenyu.top

[G05] 继承
来源：http://elf.nwbrower.top

Py:   class Admin(User): pass
来源：http://csz.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://ucq.hnqzz.top

JS:   class Admin extends User {}
来源：http://mvg.guowangkeji.top

TS:   class Admin extends User {}
来源：http://dai.gotoacloud.top

Java: class Admin extends User {}
来源：http://ono.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dzx.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://tdp.bbcook.cn

C#:   class Admin : User {}
来源：http://tqu.hysaishi.cn

[G06] 重写方法
来源：http://ewe.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://mzp.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://vdh.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://rjv.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://yte.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://fwx.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rbm.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://ucz.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://bmr.daxiang520.top

[G07] 调用父类方法
来源：http://yvy.gotoacloud.top

Py:   super().greet()
来源：http://vzp.gotoacloud.top

PHP:  parent::greet();
来源：http://ymo.yangfankeji.com

JS:   super.greet();
来源：http://udg.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://pmc.hnqzz.top

Java: super.greet();
来源：http://rcd.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://teh.fanxiaobao.xyz

Ruby: super
来源：http://jdd.nanxinkj.top

C#:   base.Greet();
来源：http://goc.nanxuanxn.top

[G08] 静态方法与属性
来源：http://fzu.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://arp.chenzaomai.com

PHP:  public static function f() {}
来源：http://fqo.9152youxi.cn

JS:   static f() {}
来源：http://lhn.zdbjq.cn

TS:   static f(): void {}
来源：http://qrq.ppjwa.cn

Java: static void f() {}
来源：http://eck.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ubv.cashguo.top

Ruby: def self.f; end
来源：http://diq.andypj.xyz

C#:   public static void F() {}
来源：http://awf.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://fzc.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://uwm.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://qsq.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://exb.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://lht.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://nfi.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://kyi.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xcx.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://ceu.jinyuanbaomall.cn

[G10] 访问控制
来源：http://tdf.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://doj.shuidangran.top

PHP:  public / protected / private
来源：http://pdk.jianghu66.top

JS:   #private 字段；其余公开
来源：http://vwx.wangdashe.top

TS:   public / protected / private
来源：http://nwt.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://rjy.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vrz.sysykeji.top

Ruby: public / protected / private
来源：http://ktu.hysaishi.cn

C#:   public / protected / private / internal
来源：http://nxd.smart0.xyz

[G11] getter / setter
来源：http://ktn.andypj.xyz

Py:   @property 与 @x.setter
来源：http://xnp.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://rem.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://fzo.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://yny.shzxlz.cn

Java: public String getName() { return name; }
来源：http://asa.hammf.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://avz.xuanzx.com

Ruby: attr_accessor :name
来源：http://xom.tanke756.top

C#:   public string Name { get; set; }
来源：http://rgl.jinqigufen.top

[G12] 对象转字符串
来源：http://trj.yj20258.top

Py:   def __str__(self): return self.name
来源：http://xfc.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xhm.cucudq.cn

JS:   toString() { return this.name; }
来源：http://azj.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://daa.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://vse.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://utu.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://yhf.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://zij.cdnleiting.top

[G13] 判断对象类型
来源：http://fww.ehwqpu.com

Py:   isinstance(u, User)
来源：http://mgd.yvedp.cn

PHP:  $u instanceof User
来源：http://pns.yongpay.top

JS:   u instanceof User
来源：http://ipm.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://oym.zhoulong.xyz

Java: u instanceof User
来源：http://ttl.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://juh.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://guc.cashguo.top

C#:   u is User
来源：http://ohg.xinyue.icu

[G14] 数据类 / record
来源：http://uas.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fpq.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://hsy.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://tva.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://wpl.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://bfy.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://dnc.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://izk.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://acl.epnwcf.com

[G15] 枚举
来源：http://yhx.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pue.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zev.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uro.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qex.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://dff.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lbn.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://pss.xuetiantiany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://neo.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://smc.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ath.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://whn.mhx1999.top

JS:   Object.entries(obj)
来源：http://vds.cucudq.cn

TS:   Object.entries(obj)
来源：http://xnu.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uea.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://toc.wangshuangyany.cn

Ruby: obj.instance_variables
来源：http://acw.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://qwa.yuanzhike.top

================================================================================
来源：http://pja.bbcook.cn

H. 异常与错误处理
来源：http://pie.xziqi.cn

================================================================================
来源：http://tpk.hcnkem.com

[H01] try / catch 基础
来源：http://gpc.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zsn.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dhi.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://skv.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kgf.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bxn.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lrr.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgy.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pxw.hnqzz.top

[H02] finally / ensure 收尾
来源：http://tqh.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://jvw.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vze.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://hrr.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dad.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ycw.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vzb.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://jid.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cye.ppjwa.cn

[H03] 主动抛出异常
来源：http://zkg.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://mfu.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cdm.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://saj.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://xlj.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lsv.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tle.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gts.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://pfd.yuanzhike.top

[H04] 自定义异常类型
来源：http://skt.cashguo.top

Py:   class MyError(Exception): pass
来源：http://xxj.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://owb.hammf.cn

JS:   class MyError extends Error {}
来源：http://hch.guannengcc.top

TS:   class MyError extends Error {}
来源：http://eop.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://mzv.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qsm.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://wtd.tarul.cn

C#:   class MyException : Exception {}
来源：http://wmo.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://xfh.tanke756.top

Py:   except ValueError as e:
来源：http://vhx.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zra.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://dnj.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://pjp.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://xcp.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hil.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://ftr.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://odu.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://drv.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://msn.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cyu.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rsb.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tyx.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qbq.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pma.shangyingyoupin.top

Ruby: d&.dig(:a, :b)
来源：http://opp.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://bex.ywan-chungtsiang.top

[H07] 断言
来源：http://muy.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://eog.jianghu66.top

PHP:  assert($x > 0);
来源：http://knf.birdmap.top

JS:   console.assert(x > 0);
来源：http://xha.tarul.cn

TS:   console.assert(x > 0);
来源：http://uhh.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://gyh.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ztf.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://pce.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://yyo.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://uns.shangyingyoupin.top

Py:   str(e);  traceback.format_exc()
来源：http://sgm.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nwf.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://hrz.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://onl.sysykeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vsw.jqgfzy.top

Go:   err.Error()
来源：http://aph.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://ojs.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://nco.jinqigfzy.top

[H09] 带错误码的异常
来源：http://rok.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nbb.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cll.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nfq.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xjq.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xei.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aus.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://amq.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fgo.dianchejie.cn

[H10] 资源自动释放
来源：http://kir.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cfk.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sus.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cwa.hesvh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ftr.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mmn.shuidangran.top

Go:   defer f.Close()
来源：http://pmw.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gyl.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://teq.ydzc1.top

================================================================================
来源：http://rkw.yj20258.top

I. 正则表达式
来源：http://gbr.birdmap.top

================================================================================
来源：http://guy.tianlin.xyz

[I01] 判断是否匹配
来源：http://lkm.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mpm.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eot.jianghu66.top

JS:   /\d+/.test(s)
来源：http://izd.aizwys.cn

TS:   /\d+/.test(s)
来源：http://gtl.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vkz.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://syw.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://peb.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gtt.smart0.xyz

[I02] 提取所有匹配
来源：http://dtb.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://fsh.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://abw.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wim.yfazqb.com

TS:   s.match(/\d+/g)
来源：http://ybm.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sfj.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gor.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://qgs.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mzb.cheryme.top

[I03] 提取捕获分组
来源：http://jww.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pkz.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vmc.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hqf.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://usm.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hgf.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gld.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://krh.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pag.yueranfly.top

[I04] 正则替换
来源：http://gdy.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kpu.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tro.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://dux.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://tos.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://fmq.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://coq.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://npy.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ghu.fktsv.cn

[I05] 按正则拆分
来源：http://muc.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nxn.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yzy.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://ctn.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://kkd.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://xus.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fry.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://yoy.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pln.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vzs.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jbg.yvedp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dtw.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qek.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://buj.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dsc.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kxc.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://amu.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nei.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://sry.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tce.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qwz.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mvw.cashguo.top

TS:   /error/gim
来源：http://ljw.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://duq.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mqo.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://pjy.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ovn.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://ktm.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://log.bjfxy.top


<!-- 参考信息 -->
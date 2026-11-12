代发 wailian999

================================================================================
来源：http://pxp.jianghu66.top

G. 面向对象
来源：http://jeo.9152youxi.cn

================================================================================
来源：http://gmj.fktsv.cn

[G01] 定义类
来源：http://kmh.epnwcf.com

Py:   class User: pass
来源：http://uxj.redwolf501.top

PHP:  class User {}
来源：http://ywy.feifeiyinyue.top

JS:   class User {}
来源：http://has.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://cmn.jinghuilouyu.cn

Java: class User {}
来源：http://own.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://dmo.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://ezy.xziqi.cn

C#:   class User {}
来源：http://vbl.cdnleiting.top

[G02] 构造函数
来源：http://tra.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://uqr.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://qsf.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://zdm.sweek.top

TS:   constructor(public name: string) {}
来源：http://kqd.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://yao.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ccr.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://lvr.zhoulong.xyz

C#:   public User(string name) { Name = name; }
来源：http://xdy.gotoacloud.top

[G03] 实例属性
来源：http://egv.tianlin.xyz

Py:   self.name = "x"
来源：http://dfy.uphjek.com

PHP:  public string $name = "x";
来源：http://jat.xylfe.cn

JS:   this.name = "x";
来源：http://icf.zhoulong.xyz

TS:   name: string = "x";
来源：http://zlx.shanyushiyangtech.top

Java: private String name;
来源：http://vtl.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yla.zdqjudy.top

Ruby: @name = "x"
来源：http://epc.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://bvc.zhengqikj.top

[G04] 定义方法
来源：http://ufg.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://chn.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://buk.daria6918.cn

JS:   greet() { return this.name; }
来源：http://eii.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://lxx.quarkkingdee.top

Java: String greet() { return name; }
来源：http://khb.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://apf.jinqigufen.top

Ruby: def greet; @name; end
来源：http://gpc.epnwcf.com

C#:   public string Greet() => Name;
来源：http://hnj.sysykeji.top

[G05] 继承
来源：http://yvp.haohaochexian.top

Py:   class Admin(User): pass
来源：http://zhx.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://yoy.redwolf501.top

JS:   class Admin extends User {}
来源：http://osc.jiagoushi.top

TS:   class Admin extends User {}
来源：http://jjz.aizwys.cn

Java: class Admin extends User {}
来源：http://rak.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xih.cdnleiting.top

Ruby: class Admin < User; end
来源：http://vmp.zhijiandao.cn

C#:   class Admin : User {}
来源：http://ovf.zdqjudy.top

[G06] 重写方法
来源：http://syc.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://rjk.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sgf.havefunace.top

JS:   greet() { return "admin"; }
来源：http://nfs.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://kql.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://lfc.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sma.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://hls.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://zzm.bjfxy.top

[G07] 调用父类方法
来源：http://hou.nanxinkj.top

Py:   super().greet()
来源：http://iqn.snrcjt.cn

PHP:  parent::greet();
来源：http://quo.zhiwuduotai.top

JS:   super.greet();
来源：http://his.zhongyouzk.top

TS:   super.greet();
来源：http://hnf.xingfuxueyuan.xyz

Java: super.greet();
来源：http://agd.jqgfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ywx.zhiwuduotai.top

Ruby: super
来源：http://rbr.cheryme.top

C#:   base.Greet();
来源：http://rfj.tian-w.cn

[G08] 静态方法与属性
来源：http://ebv.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vro.yj20258888.top

PHP:  public static function f() {}
来源：http://cwy.tanke756.top

JS:   static f() {}
来源：http://lnu.zhengqikj.top

TS:   static f(): void {}
来源：http://tbo.fengsongda.top

Java: static void f() {}
来源：http://jgc.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://osp.cucudq.cn

Ruby: def self.f; end
来源：http://efv.sysykeji.top

C#:   public static void F() {}
来源：http://com.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://ufw.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://sst.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://aws.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://way.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://cxo.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://vmc.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://nbe.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zsh.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://jsn.hnxiangtu.top

[G10] 访问控制
来源：http://vwv.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://ido.tanke756.top

PHP:  public / protected / private
来源：http://yrh.nwbrower.top

JS:   #private 字段；其余公开
来源：http://qcy.hammf.cn

TS:   public / protected / private
来源：http://fyj.yongpay.top

Java: public / protected / private / 默认包级
来源：http://qdg.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://wfl.zhiwuduotai.top

Ruby: public / protected / private
来源：http://nnp.aizwys.cn

C#:   public / protected / private / internal
来源：http://xxv.zhiwuduotai.top

[G11] getter / setter
来源：http://nmc.sxryk.cn

Py:   @property 与 @x.setter
来源：http://rls.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hcy.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://cxo.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://yha.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://zok.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://obd.guowangkeji.top

Ruby: attr_accessor :name
来源：http://nfu.nwbrower.top

C#:   public string Name { get; set; }
来源：http://ugq.ehwqpu.com

[G12] 对象转字符串
来源：http://ybc.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://ahm.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gkv.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://pae.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://yal.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://xxu.shanyushiyangtech.top

Go:   func (u User) String() string { return u.Name }
来源：http://aay.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://ndj.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://mjd.fengsongda.top

[G13] 判断对象类型
来源：http://eso.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://xvh.shzxlz.cn

PHP:  $u instanceof User
来源：http://rmy.jinqigufen.top

JS:   u instanceof User
来源：http://efr.mhx1999.top

TS:   u instanceof User
来源：http://qnu.zhongyouzk.top

Java: u instanceof User
来源：http://zpb.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hoe.tarul.cn

Ruby: u.is_a?(User)
来源：http://rfn.fanxiaobao.xyz

C#:   u is User
来源：http://zgs.gzhubu.top

[G14] 数据类 / record
来源：http://paz.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wfh.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://bkc.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://wsl.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://rrd.daxiang520.top

Java: record User(String name, int age) {}
来源：http://sce.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://att.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vzs.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://oqq.daria6918.cn

[G15] 枚举
来源：http://kgt.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mug.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://pzt.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oxm.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yvg.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://oyv.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vzn.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://nhv.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://llm.cucudq.cn

[G16] 对象转数组 / 字典
来源：http://tdz.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kkg.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://pyi.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://qlt.yuanzhike.top

TS:   Object.entries(obj)
来源：http://ujx.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://afq.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jth.jinqigufen.top

Ruby: obj.instance_variables
来源：http://rzd.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://jog.shangyingyoupin.top

================================================================================
来源：http://xun.jinqigufen.top

H. 异常与错误处理
来源：http://alj.tian-w.cn

================================================================================
来源：http://nvw.cdnleiting.top

[H01] try / catch 基础
来源：http://ktl.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rrr.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://icj.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bck.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aux.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pzl.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yhd.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hgt.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ojd.fehbvm.com

[H02] finally / ensure 收尾
来源：http://mmx.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xwa.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ivi.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://vmd.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://shv.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ezv.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://ofd.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://spv.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wcz.zhixingplan.top

[H03] 主动抛出异常
来源：http://lfc.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://dmc.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gjc.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://gfw.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://fjr.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tkf.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hbd.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://xzw.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://qpt.bbcook.cn

[H04] 自定义异常类型
来源：http://srf.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://lnn.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://jap.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://nsm.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://eii.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://hdq.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bqy.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://ngn.jianghu66.top

C#:   class MyException : Exception {}
来源：http://jgy.jlsjyb.cn

[H05] 捕获特定类型
来源：http://soi.jianghu66.top

Py:   except ValueError as e:
来源：http://cds.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xop.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://ioo.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://axc.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://qzb.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://otz.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://zai.hywenlv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kws.vehdjk.com

[H06] 可选值 / 空值安全访问
来源：http://xqk.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://mfd.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yvi.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://mtz.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qau.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zpc.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ulh.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://jzh.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://sea.zhiwuduotai.top

[H07] 断言
来源：http://ehy.ydzc1.top

Py:   assert x > 0, "必须为正"
来源：http://zzm.fzhhl.top

PHP:  assert($x > 0);
来源：http://awv.shuidangran.top

JS:   console.assert(x > 0);
来源：http://gsh.daria6918.cn

TS:   console.assert(x > 0);
来源：http://koo.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://yjh.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mfs.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wje.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://sva.jiagoushi.top

[H08] 获取错误信息与堆栈
来源：http://uxr.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://unx.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vco.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://jyd.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vem.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vdu.yongpay.top

Go:   err.Error()
来源：http://bob.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://bal.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://igk.xziqi.cn

[H09] 带错误码的异常
来源：http://tfe.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qtg.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://vvx.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zfp.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ofj.316326.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fvu.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jzg.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://ymm.redwolf501.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hyj.yuxming.cn

[H10] 资源自动释放
来源：http://piw.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://inr.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kuv.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bly.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rvg.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tkt.gzhubu.top

Go:   defer f.Close()
来源：http://bca.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vho.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rjg.xylfe.cn

================================================================================
来源：http://lur.dianchejie.cn

I. 正则表达式
来源：http://wyt.sjlbkw.cn

================================================================================
来源：http://wog.ydjk.org.cn

[I01] 判断是否匹配
来源：http://gsg.sjlbkw.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://roy.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://isy.uphjek.com

JS:   /\d+/.test(s)
来源：http://lfb.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://nyk.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nkq.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ojo.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://itu.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wfc.jiagoushi.top

[I02] 提取所有匹配
来源：http://yqx.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://tvw.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kor.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kud.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://zlp.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dnw.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://osv.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://vwy.316326.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jma.bbcook.cn

[I03] 提取捕获分组
来源：http://uxm.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dpe.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dma.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybx.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://usn.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ejf.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tbb.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gqu.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nwy.sysykeji.top

[I04] 正则替换
来源：http://lst.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yql.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aqu.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://hgx.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://tso.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://bsm.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hzj.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cei.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rnv.jinghuilouyu.cn

[I05] 按正则拆分
来源：http://fuv.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yiv.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://upj.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://vii.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://xpy.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://amq.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://moe.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://dmt.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qnd.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ahp.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://liz.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sks.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tgx.ivvv.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rrf.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gva.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xgg.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qnx.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qha.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://qnn.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vkq.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vwq.jqgufenzy.top


<!-- 参考信息 -->
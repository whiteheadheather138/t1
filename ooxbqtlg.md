代发 wailian999

TS:   constructor(public name: string) {}
来源：http://deh.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://edn.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vkl.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://tyh.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://pfy.sweek.top

[G03] 实例属性
来源：http://enn.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://imq.daxiang520.top

PHP:  public string $name = "x";
来源：http://jdy.tianlin.xyz

JS:   this.name = "x";
来源：http://yep.chenjidiqi.icu

TS:   name: string = "x";
来源：http://vtc.9152youxi.cn

Java: private String name;
来源：http://fen.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xzh.yj20258888.top

Ruby: @name = "x"
来源：http://jvt.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://wfl.cheryme.top

[G04] 定义方法
来源：http://wpe.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://edy.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://elh.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://akq.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://lbf.sjlbkw.cn

Java: String greet() { return name; }
来源：http://cbj.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vmg.wangshuangyany.cn

Ruby: def greet; @name; end
来源：http://nce.nwbrower.top

C#:   public string Greet() => Name;
来源：http://drc.jianghu66.top

[G05] 继承
来源：http://bqa.gogol.net.cn

Py:   class Admin(User): pass
来源：http://ctk.yj20258888.top

PHP:  class Admin extends User {}
来源：http://qom.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://urt.ivvv.top

TS:   class Admin extends User {}
来源：http://dbp.shanyushiyangkeji.top

Java: class Admin extends User {}
来源：http://ezp.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hhw.yuanzhike.top

Ruby: class Admin < User; end
来源：http://fhj.ydzc1.top

C#:   class Admin : User {}
来源：http://fcd.zhixingplan.top

[G06] 重写方法
来源：http://zip.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://vec.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fry.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://rtw.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://nde.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://dil.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sxt.gzhubu.top

Ruby: def greet; "admin"; end
来源：http://aod.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://pjy.sysykeji.top

[G07] 调用父类方法
来源：http://rxc.nwbrower.top

Py:   super().greet()
来源：http://cbv.yj20258888.top

PHP:  parent::greet();
来源：http://xdz.tian-w.cn

JS:   super.greet();
来源：http://fhs.jqgfzy.top

TS:   super.greet();
来源：http://ecs.aizwys.cn

Java: super.greet();
来源：http://ucv.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bbg.hywenlv.cn

Ruby: super
来源：http://hjk.yvedp.cn

C#:   base.Greet();
来源：http://oay.tianlin.xyz

[G08] 静态方法与属性
来源：http://opc.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://akp.gaohongyu789.top

PHP:  public static function f() {}
来源：http://uzv.haohaochexian.top

JS:   static f() {}
来源：http://gza.meibo888.top

TS:   static f(): void {}
来源：http://ash.jianghu66.top

Java: static void f() {}
来源：http://txw.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://feo.hongshengwenyu.top

Ruby: def self.f; end
来源：http://xhl.cucudq.cn

C#:   public static void F() {}
来源：http://cdw.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://fgw.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://uje.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://eho.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://llo.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://xzc.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://abw.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://usy.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cqk.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://yla.yj20258888.top

[G10] 访问控制
来源：http://elz.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://zvk.tianlin.xyz

PHP:  public / protected / private
来源：http://tnr.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://uao.zhongyouzk.top

TS:   public / protected / private
来源：http://tfr.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://xoy.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://evq.9152youxi.cn

Ruby: public / protected / private
来源：http://xzn.hammf.cn

C#:   public / protected / private / internal
来源：http://btx.guowangkeji.top

[G11] getter / setter
来源：http://fic.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://dgo.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xle.sysykeji.top

JS:   get name() { return this._name; }
来源：http://mlf.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://wgo.uphjek.com

Java: public String getName() { return name; }
来源：http://fzv.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ogh.52xcode.cn

Ruby: attr_accessor :name
来源：http://ffi.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://yir.nanxinkj.top

[G12] 对象转字符串
来源：http://omq.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://mqm.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://hcv.uphjek.com

JS:   toString() { return this.name; }
来源：http://gcn.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://pqg.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://ztc.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://dmh.cashguo.top

Ruby: def to_s; @name; end
来源：http://hzg.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://hji.52xcode.cn

[G13] 判断对象类型
来源：http://whp.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://mfr.c1oappe.top

PHP:  $u instanceof User
来源：http://ndn.feifeiyinyue.top

JS:   u instanceof User
来源：http://vvw.gogol.net.cn

TS:   u instanceof User
来源：http://lfn.tian-w.cn

Java: u instanceof User
来源：http://cmk.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://irb.cheryme.top

Ruby: u.is_a?(User)
来源：http://xqj.aibaodan.cn

C#:   u is User
来源：http://kvm.dashuyun.cn

[G14] 数据类 / record
来源：http://mky.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lmj.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://toa.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vma.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://dtb.zhixingplan.top

Java: record User(String name, int age) {}
来源：http://bpm.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://lau.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rqj.ydzc1.top

C#:   record User(string Name, int Age);
来源：http://ihx.wangdashe.top

[G15] 枚举
来源：http://thl.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hsp.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://buk.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mmk.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dzc.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://cai.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pix.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://mrg.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mfc.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://tjf.haohaochexian.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ysg.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://hdd.fehbvm.com

JS:   Object.entries(obj)
来源：http://amd.nwbrower.top

TS:   Object.entries(obj)
来源：http://utj.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://puh.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jci.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://fxi.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://hji.tianlin.xyz

================================================================================
来源：http://cfp.shuidangran.top

H. 异常与错误处理
来源：http://gwx.xuanzx.com

================================================================================
来源：http://dga.havefunace.top

[H01] try / catch 基础
来源：http://vsm.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hfv.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://irk.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://loo.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hnv.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://acp.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xtx.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wop.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pyd.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://otr.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://olu.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yce.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://loo.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://jsv.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://ksg.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xcz.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uln.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aog.yongpay.top

[H03] 主动抛出异常
来源：http://ljz.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://ytf.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rhg.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://qln.ivvv.top

TS:   throw new Error("错误信息");
来源：http://sbu.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://hta.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lbk.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zgo.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://aga.ydjk.org.cn

[H04] 自定义异常类型
来源：http://azf.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://bex.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://piw.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://dbz.redwolf501.top

TS:   class MyError extends Error {}
来源：http://oeo.hongshengwenyu.top

Java: class MyException extends RuntimeException {}
来源：http://iyh.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uuv.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://spr.gzhubu.top

C#:   class MyException : Exception {}
来源：http://dap.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://ljf.zhongyouzk.top

Py:   except ValueError as e:
来源：http://rbv.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ygm.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://ips.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://lzt.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://fbj.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blv.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://mno.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lfp.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://qkc.316326.xyz

Py:   value = d.get("k") or default
来源：http://xgc.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://nic.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://xmq.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kjs.jqgfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wim.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yfk.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://dza.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://klu.cqqwz.cn

[H07] 断言
来源：http://etx.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://zsm.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://yok.hesvh.cn

JS:   console.assert(x > 0);
来源：http://cfu.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://wsa.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://ydp.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zcg.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://yun.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://hjc.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://szt.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://aqu.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://icg.fehbvm.com

JS:   e.message;  e.stack
来源：http://hns.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nrk.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jak.wangshuangyany.cn

Go:   err.Error()
来源：http://lbo.quarkkingdee.top

Ruby: e.message;  e.backtrace
来源：http://ofv.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://uil.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://ptf.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://grw.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fln.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bbh.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xob.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://amc.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zlz.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://uow.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ypo.c1oappe.top

[H10] 资源自动释放
来源：http://uif.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hql.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cvx.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wfy.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pta.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lpr.zhiwuduotai.top

Go:   defer f.Close()
来源：http://tjw.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hbw.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gmb.fzhhl.top

================================================================================
来源：http://psv.nwbrower.top

I. 正则表达式
来源：http://fxr.xinyue.icu

================================================================================
来源：http://xzy.0kj1m.cn

[I01] 判断是否匹配
来源：http://nvp.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://udt.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://oza.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://ivx.meibo888.top

TS:   /\d+/.test(s)
来源：http://bkw.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jst.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ryi.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://vwq.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oys.birdmap.top

[I02] 提取所有匹配
来源：http://zoo.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://csa.tianlin.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vnc.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xnl.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://dbn.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aqa.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mzs.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://gct.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vlz.fktsv.cn

[I03] 提取捕获分组
来源：http://ndm.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://htm.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ywo.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lsb.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oxn.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jbp.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://okv.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pje.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vgk.wangdashe.top

[I04] 正则替换
来源：http://mlx.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sbe.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://you.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://akf.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://olr.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://amm.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://rce.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://klj.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rwz.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://xuo.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://tcx.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wrg.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ijg.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://phj.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://ktr.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qll.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://rbl.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rmz.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zag.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://djw.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hnk.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gjx.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ieh.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pzu.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kks.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rma.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hxc.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://uzj.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ppk.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oss.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gkr.hnqzz.top

TS:   /error/gim
来源：http://waw.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zvy.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xts.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://aif.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jvv.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://jfn.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xwx.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vqv.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://asb.yj20258.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ydj.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qro.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zrr.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tit.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tad.shanyushiyangkeji.top

================================================================================
来源：http://sjy.wangdashe.top


<!-- 参考信息 -->
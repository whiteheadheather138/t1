代发 wailian999

[G02] 构造函数
来源：http://sqz.bjfxy.top

Py:   def __init__(self, name): self.name = name
来源：http://lnt.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://ycr.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://bjr.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://mqt.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://kon.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tzw.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://phr.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://qxz.bjfxy.top

[G03] 实例属性
来源：http://wov.zhixingplan.top

Py:   self.name = "x"
来源：http://uge.jinqigufen.top

PHP:  public string $name = "x";
来源：http://see.wangshuangyany.cn

JS:   this.name = "x";
来源：http://jhw.gotoacloud.top

TS:   name: string = "x";
来源：http://aso.ppjwa.cn

Java: private String name;
来源：http://doc.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qqw.cucudq.cn

Ruby: @name = "x"
来源：http://pil.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://cul.snrcjt.cn

[G04] 定义方法
来源：http://qra.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://kxj.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jbj.hesvh.cn

JS:   greet() { return this.name; }
来源：http://wwf.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://dva.ctjpmb.com

Java: String greet() { return name; }
来源：http://qlq.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cll.redwolf501.top

Ruby: def greet; @name; end
来源：http://wvu.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://wqn.yueranfly.top

[G05] 继承
来源：http://gdr.fktsv.cn

Py:   class Admin(User): pass
来源：http://ovc.fktsv.cn

PHP:  class Admin extends User {}
来源：http://oge.redwolf501.top

JS:   class Admin extends User {}
来源：http://edh.nwbrower.top

TS:   class Admin extends User {}
来源：http://xfu.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://uae.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iry.zhixingplan.top

Ruby: class Admin < User; end
来源：http://gzl.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://ptn.zhoulong.xyz

[G06] 重写方法
来源：http://uqr.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://kkf.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lzo.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://fzp.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://aoa.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://nys.jinyuanbaomall.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xpo.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://que.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://vzy.vqdsnc.cn

[G07] 调用父类方法
来源：http://huz.fktsv.cn

Py:   super().greet()
来源：http://twx.zycfv.cn

PHP:  parent::greet();
来源：http://ese.jqgufenzy.top

JS:   super.greet();
来源：http://ijc.gotoacloud.top

TS:   super.greet();
来源：http://jtv.hongshengwenyu.top

Java: super.greet();
来源：http://jgk.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://etw.xziqi.cn

Ruby: super
来源：http://ggj.pengpengdd.cyou

C#:   base.Greet();
来源：http://nhb.kuanghao11.cn

[G08] 静态方法与属性
来源：http://gct.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tvw.tarul.cn

PHP:  public static function f() {}
来源：http://ski.316326.xyz

JS:   static f() {}
来源：http://zmn.gogol.net.cn

TS:   static f(): void {}
来源：http://vvo.yj20258.top

Java: static void f() {}
来源：http://akx.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qvk.wangshuangyany.cn

Ruby: def self.f; end
来源：http://xrd.tarul.cn

C#:   public static void F() {}
来源：http://xpa.vehdjk.com

[G09] 接口 / 抽象类
来源：http://kid.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://efn.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xhb.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jff.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://sml.xziqi.cn

Java: interface Shape { double area(); }
来源：http://uye.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://lre.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bio.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://ycr.zdqjudy.top

[G10] 访问控制
来源：http://rlm.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://ubx.52xcode.cn

PHP:  public / protected / private
来源：http://ljf.havefunace.top

JS:   #private 字段；其余公开
来源：http://bsm.zdqjudy.top

TS:   public / protected / private
来源：http://tsg.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://ace.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rof.yj202588.top

Ruby: public / protected / private
来源：http://jqb.fehbvm.com

C#:   public / protected / private / internal
来源：http://box.fehbvm.com

[G11] getter / setter
来源：http://bvt.sxryk.cn

Py:   @property 与 @x.setter
来源：http://slp.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lgq.xylfe.cn

JS:   get name() { return this._name; }
来源：http://epg.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://uha.zdqjudy.top

Java: public String getName() { return name; }
来源：http://jff.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rhm.chenlongwang.top

Ruby: attr_accessor :name
来源：http://krg.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://sil.tarul.cn

[G12] 对象转字符串
来源：http://lbr.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://ema.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xaz.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://oov.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://mjx.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://ecc.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kmj.cucudq.cn

Ruby: def to_s; @name; end
来源：http://njh.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://ieh.zhoulong.xyz

[G13] 判断对象类型
来源：http://vha.cheryme.top

Py:   isinstance(u, User)
来源：http://fgj.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://ifb.cucudq.cn

JS:   u instanceof User
来源：http://gsj.ctjpmb.com

TS:   u instanceof User
来源：http://gon.jlsjyb.cn

Java: u instanceof User
来源：http://rkg.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hyk.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://gxj.jinyuanbaomall.cn

C#:   u is User
来源：http://kkh.bjfxy.top

[G14] 数据类 / record
来源：http://qrj.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xdj.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://mde.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://aud.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://xjy.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://ipw.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://ooa.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cxt.birdmap.top

C#:   record User(string Name, int Age);
来源：http://xxe.ydzc1.top

[G15] 枚举
来源：http://sdt.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://otf.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://psb.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mxq.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hsr.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://ihy.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nte.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://hme.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ciz.sweek.top

[G16] 对象转数组 / 字典
来源：http://npa.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ssy.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://cyc.hesvh.cn

JS:   Object.entries(obj)
来源：http://dtt.uphjek.com

TS:   Object.entries(obj)
来源：http://ctz.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eph.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://rvq.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://wqk.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://voc.yuxming.cn

================================================================================
来源：http://upv.tanke756.top

H. 异常与错误处理
来源：http://hck.hongshengwenyu.top

================================================================================
来源：http://onw.hfpthk.cn

[H01] try / catch 基础
来源：http://ddp.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uub.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vqr.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oyx.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nwo.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hcq.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wcg.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zer.smart0.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ubq.hnqzz.top

[H02] finally / ensure 收尾
来源：http://mjf.yueranfly.top

Py:   try: f()⏎finally: cleanup()
来源：http://fgg.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sxn.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://kpw.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ihd.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://lxz.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ven.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ikn.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://olb.sjlbkw.cn

[H03] 主动抛出异常
来源：http://qhw.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://yzd.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://djh.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://pwm.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://wwd.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://awf.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bef.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ozb.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tnz.quarkkingdee.top

[H04] 自定义异常类型
来源：http://shx.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://eoh.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://uxr.shuidangran.top

JS:   class MyError extends Error {}
来源：http://fbr.yfazqb.com

TS:   class MyError extends Error {}
来源：http://bhj.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://sxh.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vdn.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://jik.iojbl.cn

C#:   class MyException : Exception {}
来源：http://gcn.nwbrower.top

[H05] 捕获特定类型
来源：http://lfe.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://mih.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ubb.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://xob.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://mtu.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://ote.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ezc.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://iue.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cpa.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://xfr.daxiang520.top

Py:   value = d.get("k") or default
来源：http://dko.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vrc.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://sam.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://tbv.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zqv.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uid.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://xwx.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://kxd.hysaishi.cn

[H07] 断言
来源：http://blp.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://hyw.zhengqikj.top

PHP:  assert($x > 0);
来源：http://oyg.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://mtq.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://gic.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://plz.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rdf.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://uhj.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://rfi.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://ehy.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://gub.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pdw.ydzc1.top

JS:   e.message;  e.stack
来源：http://vju.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uvi.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rwf.smart0.xyz

Go:   err.Error()
来源：http://vze.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://grw.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://ofw.chenlongwang.top

[H09] 带错误码的异常
来源：http://fdu.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://apu.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://swz.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qrt.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cpg.jianghu66.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dlo.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ckc.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://iph.chenjidiqi.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://bzc.feifeiyinyue.top

[H10] 资源自动释放
来源：http://nof.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ugg.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ptu.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xsz.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vqd.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iep.xuetiantiany.cn

Go:   defer f.Close()
来源：http://ktl.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eyr.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://smk.birdmap.top

================================================================================
来源：http://jsm.hysaishi.cn

I. 正则表达式
来源：http://nlt.cqqwz.cn

================================================================================
来源：http://zgr.yvedp.cn

[I01] 判断是否匹配
来源：http://rrn.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://inn.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://roo.yangfankeji.com

JS:   /\d+/.test(s)
来源：http://qsm.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://jud.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cke.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xjt.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://chy.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://okd.xziqi.cn

[I02] 提取所有匹配
来源：http://ote.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://abt.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kqj.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tee.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://wyp.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ndp.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gvh.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://woo.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ibv.xziqi.cn

[I03] 提取捕获分组
来源：http://rvv.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tdr.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://txm.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://okx.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vbk.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ahn.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bsz.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vne.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://emw.hnxiangtu.top

[I04] 正则替换
来源：http://xqf.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gfy.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bog.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://bcf.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hpo.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://lff.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cvq.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://csi.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ggf.smart0.xyz

[I05] 按正则拆分
来源：http://mkl.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iaf.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://unb.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://pdb.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://rdd.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://ftc.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tbn.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vhr.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eri.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lsa.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hwz.yvedp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bsk.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lvs.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://siw.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tcd.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ehu.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ibq.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lcx.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://tgn.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://plu.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xem.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cww.hesvh.cn

TS:   /error/gim
来源：http://oty.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xob.tanke756.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yjc.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://foh.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://adq.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://hhq.hcnkem.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://edn.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hat.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yyf.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ylo.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://edr.ywan-chungtsiang.top


<!-- 参考信息 -->
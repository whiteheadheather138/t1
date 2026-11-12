代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hdq.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://kmq.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pxc.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://eui.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://oec.nanxuanxn.top

[G03] 实例属性
来源：http://hoi.hesvh.cn

Py:   self.name = "x"
来源：http://vbn.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://mwq.tanke756.top

JS:   this.name = "x";
来源：http://eab.cdnleiting.top

TS:   name: string = "x";
来源：http://daw.sjlbkw.cn

Java: private String name;
来源：http://gts.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bno.yj20258.top

Ruby: @name = "x"
来源：http://edm.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://cfz.ehwqpu.com

[G04] 定义方法
来源：http://pjh.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://prt.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nxa.fktsv.cn

JS:   greet() { return this.name; }
来源：http://odw.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://arn.ehwqpu.com

Java: String greet() { return name; }
来源：http://nhn.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://hth.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://uoe.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://lqd.jianghu66.top

[G05] 继承
来源：http://pge.bbcook.cn

Py:   class Admin(User): pass
来源：http://vrm.guannengcc.top

PHP:  class Admin extends User {}
来源：http://pit.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://xbz.hesvh.cn

TS:   class Admin extends User {}
来源：http://xjn.nanxinkj.top

Java: class Admin extends User {}
来源：http://qks.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cpr.cucudq.cn

Ruby: class Admin < User; end
来源：http://gcv.vehdjk.com

C#:   class Admin : User {}
来源：http://ark.hcnkem.com

[G06] 重写方法
来源：http://ikx.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://euz.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://veh.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://zxs.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://zbz.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://con.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oht.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://apb.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://him.yuanzhike.top

[G07] 调用父类方法
来源：http://itd.pycfn.com

Py:   super().greet()
来源：http://ivx.zhengqikj.top

PHP:  parent::greet();
来源：http://btt.gotoacloud.top

JS:   super.greet();
来源：http://fpt.ywan-chungtsiang.top

TS:   super.greet();
来源：http://txx.ydjk.org.cn

Java: super.greet();
来源：http://jup.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wsj.cucudq.cn

Ruby: super
来源：http://cqh.aibaodan.cn

C#:   base.Greet();
来源：http://vry.gaohongyu789.top

[G08] 静态方法与属性
来源：http://tum.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vot.ehwqpu.com

PHP:  public static function f() {}
来源：http://gsi.9152youxi.cn

JS:   static f() {}
来源：http://lmc.xylfe.cn

TS:   static f(): void {}
来源：http://mcb.meibo888.top

Java: static void f() {}
来源：http://vmi.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oad.yuanzhike.top

Ruby: def self.f; end
来源：http://hnp.wangshuangyany.cn

C#:   public static void F() {}
来源：http://lrb.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://bnc.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://jlb.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://pix.shanyushiyangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tap.ehwqpu.com

TS:   interface Shape { area(): number; }
来源：http://ufz.pycfn.com

Java: interface Shape { double area(); }
来源：http://hzn.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://syy.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://myw.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://quq.shzxlz.cn

[G10] 访问控制
来源：http://mmj.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://zrb.zhijiandao.cn

PHP:  public / protected / private
来源：http://exc.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://mhb.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://ple.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://tdw.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jau.svipenyu.cn

Ruby: public / protected / private
来源：http://ilh.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://wgk.bjfxy.top

[G11] getter / setter
来源：http://stj.sysykeji.top

Py:   @property 与 @x.setter
来源：http://rcc.sweek.top

PHP:  public function getName(): string { return $this->name; }
来源：http://iqy.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://tea.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://sqg.hywenlv.cn

Java: public String getName() { return name; }
来源：http://nis.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ahv.hcnkem.com

Ruby: attr_accessor :name
来源：http://xbj.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://nub.epnwcf.com

[G12] 对象转字符串
来源：http://pin.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://bpq.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://khn.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://eme.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://gje.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://zsd.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hcd.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://cqc.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://ulw.uphjek.com

[G13] 判断对象类型
来源：http://mom.xziqi.cn

Py:   isinstance(u, User)
来源：http://gcc.yueranfly.top

PHP:  $u instanceof User
来源：http://rsl.jinqigfzy.top

JS:   u instanceof User
来源：http://oic.yangfankeji.com

TS:   u instanceof User
来源：http://hyc.shanyushiyangtech.top

Java: u instanceof User
来源：http://pio.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ugt.hnqzz.top

Ruby: u.is_a?(User)
来源：http://sbd.iojbl.cn

C#:   u is User
来源：http://siz.svipenyu.cn

[G14] 数据类 / record
来源：http://xpy.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iiz.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://xyr.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://gnn.jinyuanbaomall.cn

TS:   type User = { name: string; age: number };
来源：http://pty.vehdjk.com

Java: record User(String name, int age) {}
来源：http://fqd.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://xit.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iwq.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://irx.epnwcf.com

[G15] 枚举
来源：http://uke.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dvc.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ykw.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xfh.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lza.fanxiaobao.xyz

Java: enum Color { RED, GREEN }
来源：http://czl.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ufx.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://zha.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vgd.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://miw.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jwc.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://jyo.guannengcc.top

JS:   Object.entries(obj)
来源：http://mdp.jiagoushi.top

TS:   Object.entries(obj)
来源：http://qal.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://byu.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gik.c1oappe.top

Ruby: obj.instance_variables
来源：http://nmy.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://gvw.hfpthk.cn

================================================================================
来源：http://uqn.hnqzz.top

H. 异常与错误处理
来源：http://pmq.cqqwz.cn

================================================================================
来源：http://kbw.ivvv.top

[H01] try / catch 基础
来源：http://jys.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wfg.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hyh.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cer.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://evd.chenlongwang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dhr.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://imx.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nct.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rqu.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://mpf.quarkkingdee.top

Py:   try: f()⏎finally: cleanup()
来源：http://iof.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zci.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qqw.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bug.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://kxa.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gxr.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lsi.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pox.jyoumei.cn

[H03] 主动抛出异常
来源：http://uux.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://tjf.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zqd.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://icg.ivvv.top

TS:   throw new Error("错误信息");
来源：http://zte.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zec.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jal.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yto.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://kfu.hnxiangtu.top

[H04] 自定义异常类型
来源：http://hag.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://iir.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://pld.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://jwf.yj20258888.top

TS:   class MyError extends Error {}
来源：http://ieb.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://xga.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://age.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://hna.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://zqr.xuanzx.com

[H05] 捕获特定类型
来源：http://ext.aibaodan.cn

Py:   except ValueError as e:
来源：http://yvy.jiagoushi.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uwi.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://fng.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://rly.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://xtn.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wos.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://sof.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://scn.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://zly.yonumen.top

Py:   value = d.get("k") or default
来源：http://iiz.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://wax.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wnt.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://qwm.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rgy.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nmg.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://opg.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://blk.hfpthk.cn

[H07] 断言
来源：http://xxg.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://rts.yueranfly.top

PHP:  assert($x > 0);
来源：http://ehb.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://pay.ybcxt.top

TS:   console.assert(x > 0);
来源：http://wey.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://czw.ybcxt.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tqo.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://qqs.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://lit.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://pau.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://lsq.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pds.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://rzl.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wlj.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wgb.cashguo.top

Go:   err.Error()
来源：http://nlm.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://gdm.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://lun.9152youxi.cn

[H09] 带错误码的异常
来源：http://dzf.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kyg.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://oum.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nwx.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://opx.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pdu.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://apo.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://mbl.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vmy.smart0.xyz

[H10] 资源自动释放
来源：http://anx.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ifn.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tvl.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://esz.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fex.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://stx.kuanghao11.cn

Go:   defer f.Close()
来源：http://ykb.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://brx.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sgt.fanxiaobao.xyz

================================================================================
来源：http://ttf.hcnkem.com

I. 正则表达式
来源：http://elt.jlsjyb.cn

================================================================================
来源：http://otc.0kj1m.cn

[I01] 判断是否匹配
来源：http://aku.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yyy.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://waf.yj20258888.top

JS:   /\d+/.test(s)
来源：http://ckn.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://dqi.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cva.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jxt.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://wag.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iwf.zhongyouzk.top

[I02] 提取所有匹配
来源：http://mhj.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://cli.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xeg.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jkt.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://jbf.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zeo.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lxl.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://wis.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wzj.vqdsnc.cn

[I03] 提取捕获分组
来源：http://cxo.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zvb.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fwi.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zce.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nju.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jie.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tha.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://emt.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nyc.yongpay.top

[I04] 正则替换
来源：http://zjd.svipenyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jze.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://emj.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://mks.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://zqr.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://fca.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bnq.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zrv.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bct.fengsongda.top

[I05] 按正则拆分
来源：http://hcj.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://awj.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rhp.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://sjp.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://kdu.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://lzc.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xfq.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://upn.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xaj.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lqn.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dmy.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://osk.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pjv.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zvw.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pnl.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yys.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lkr.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eph.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://mvq.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tuu.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xiy.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zcz.xinyue.icu

TS:   /error/gim
来源：http://yjr.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kxr.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://quo.ivvv.top

Ruby: s.scan(/error/i)
来源：http://fpc.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xyc.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://mcv.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rty.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ceo.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hos.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://onr.haohaochexian.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://agm.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://etz.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zem.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hqd.daria6918.cn

================================================================================
来源：http://eiw.cashguo.top


<!-- 参考信息 -->
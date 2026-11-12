代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://jtv.wangshuangyany.cn

[G03] 实例属性
来源：http://fko.pengpengdd.cyou

Py:   self.name = "x"
来源：http://qow.mhx1999.top

PHP:  public string $name = "x";
来源：http://ogu.hnxiangtu.top

JS:   this.name = "x";
来源：http://rie.cashguo.top

TS:   name: string = "x";
来源：http://wio.yuanzhike.top

Java: private String name;
来源：http://jqk.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gwe.jiagoushi.top

Ruby: @name = "x"
来源：http://ohj.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://nvm.tian-w.cn

[G04] 定义方法
来源：http://pli.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://yld.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://xez.hesvh.cn

JS:   greet() { return this.name; }
来源：http://lbj.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://xoo.yanxiufei.cn

Java: String greet() { return name; }
来源：http://aod.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ypv.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://cng.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://vts.gotoacloud.top

[G05] 继承
来源：http://uvj.sufxvd.cn

Py:   class Admin(User): pass
来源：http://ttf.ybcxt.top

PHP:  class Admin extends User {}
来源：http://epw.dashuyun.cn

JS:   class Admin extends User {}
来源：http://wnz.shangyingyoupin.top

TS:   class Admin extends User {}
来源：http://pxk.ybcxt.top

Java: class Admin extends User {}
来源：http://rrs.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nfa.bjfxy.top

Ruby: class Admin < User; end
来源：http://zlm.zhoulong.xyz

C#:   class Admin : User {}
来源：http://sgj.sysykeji.top

[G06] 重写方法
来源：http://aju.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://zzn.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://fbv.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://tgg.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://xsy.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://aop.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sht.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://pgk.andypj.xyz

C#:   public override string Greet() => "admin";
来源：http://eeo.jlsjyb.cn

[G07] 调用父类方法
来源：http://qps.c1oappe.top

Py:   super().greet()
来源：http://xjv.tian-w.cn

PHP:  parent::greet();
来源：http://nml.jianghu66.top

JS:   super.greet();
来源：http://wrm.shuidangran.top

TS:   super.greet();
来源：http://plq.jyoumei.cn

Java: super.greet();
来源：http://zbh.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hkw.hcnkem.com

Ruby: super
来源：http://rww.kuanghao11.cn

C#:   base.Greet();
来源：http://sym.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://kja.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jsu.0kj1m.cn

PHP:  public static function f() {}
来源：http://emy.hcnkem.com

JS:   static f() {}
来源：http://ouy.xylfe.cn

TS:   static f(): void {}
来源：http://hfc.fehbvm.com

Java: static void f() {}
来源：http://szi.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://frg.ppjwa.cn

Ruby: def self.f; end
来源：http://lyh.ydjk.org.cn

C#:   public static void F() {}
来源：http://azo.52xcode.cn

[G09] 接口 / 抽象类
来源：http://ged.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://azs.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://txl.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hau.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://vqc.yfazqb.com

Java: interface Shape { double area(); }
来源：http://rhe.52xcode.cn

Go:   type Shape interface { Area() float64 }
来源：http://liu.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ihj.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://ymw.jqgfzy.top

[G10] 访问控制
来源：http://lvc.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://lez.yanxiufei.cn

PHP:  public / protected / private
来源：http://mys.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://mnw.smart0.xyz

TS:   public / protected / private
来源：http://ooe.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://ojt.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ntj.shzxlz.cn

Ruby: public / protected / private
来源：http://qqz.cdnleiting.top

C#:   public / protected / private / internal
来源：http://pfs.fktsv.cn

[G11] getter / setter
来源：http://xjl.yfazqb.com

Py:   @property 与 @x.setter
来源：http://gpt.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yge.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://lmc.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://oha.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://eic.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://amj.tarul.cn

Ruby: attr_accessor :name
来源：http://blg.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://ohp.xuanzx.com

[G12] 对象转字符串
来源：http://jwo.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://yho.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zwr.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://ubr.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://luu.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://rrb.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nto.hammf.cn

Ruby: def to_s; @name; end
来源：http://odw.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://xfs.hfpthk.cn

[G13] 判断对象类型
来源：http://muu.xuanzx.com

Py:   isinstance(u, User)
来源：http://lmv.ydjk.org.cn

PHP:  $u instanceof User
来源：http://zim.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://smf.ctjpmb.com

TS:   u instanceof User
来源：http://cur.52xcode.cn

Java: u instanceof User
来源：http://jqn.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xmf.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://tcc.shanyushiyangkeji.top

C#:   u is User
来源：http://umz.yueranfly.top

[G14] 数据类 / record
来源：http://yut.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ozq.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://clc.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qpo.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://pms.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://ail.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://ejm.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bxk.cheryme.top

C#:   record User(string Name, int Age);
来源：http://zyk.jinqigfzy.top

[G15] 枚举
来源：http://vnj.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yjr.cucudq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iuo.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://txp.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blg.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://ftu.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tvs.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://lpq.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eos.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://bkd.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xmr.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://mbx.andypj.xyz

JS:   Object.entries(obj)
来源：http://boq.uphjek.com

TS:   Object.entries(obj)
来源：http://fdz.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://map.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ltu.redwolf501.top

Ruby: obj.instance_variables
来源：http://mon.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://qrq.hywenlv.cn

================================================================================
来源：http://stk.meibo888.top

H. 异常与错误处理
来源：http://deq.jinqigufen.top

================================================================================
来源：http://wwh.svipenyu.cn

[H01] try / catch 基础
来源：http://eal.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rez.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ykw.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iqm.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rke.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vtv.jinghuilouyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://egi.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wyr.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oph.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://ryf.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://vln.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hhf.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xxd.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jho.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eai.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://zdi.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lxj.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://hip.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://lef.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://glf.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jkk.tarul.cn

JS:   throw new Error("错误信息");
来源：http://tss.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://skw.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xlo.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ltf.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hhb.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://kik.bbcook.cn

[H04] 自定义异常类型
来源：http://hex.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://wtv.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://peh.316326.xyz

JS:   class MyError extends Error {}
来源：http://lzt.yueranfly.top

TS:   class MyError extends Error {}
来源：http://xoa.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://qnq.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uxd.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://xjl.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://yko.0kj1m.cn

[H05] 捕获特定类型
来源：http://stt.guannengcc.top

Py:   except ValueError as e:
来源：http://qmw.guowangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xky.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://htz.gogol.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://slk.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://dof.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cvs.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://oiq.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dhq.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://eqf.sxryk.cn

Py:   value = d.get("k") or default
来源：http://vod.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://agl.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://lgt.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://rkh.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hbh.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://yhm.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://ack.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://osz.hywenlv.cn

[H07] 断言
来源：http://rzy.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://gqh.havefunace.top

PHP:  assert($x > 0);
来源：http://bnd.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://pwk.sysykeji.top

TS:   console.assert(x > 0);
来源：http://hyd.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://uea.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qhg.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ddp.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://puw.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://jom.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://aaz.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wtz.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://ebx.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://lpr.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xzx.shzxlz.cn

Go:   err.Error()
来源：http://spv.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://bxm.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://ocq.meibo888.top

[H09] 带错误码的异常
来源：http://ztr.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://arq.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gnr.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cxk.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hmn.cashguo.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dlu.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iku.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://rmg.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pql.316326.xyz

[H10] 资源自动释放
来源：http://cvj.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xtd.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kpo.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wxt.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://map.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tdc.redwolf501.top

Go:   defer f.Close()
来源：http://xfx.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xke.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bkz.pengpengdd.cyou

================================================================================
来源：http://wyq.shzxlz.cn

I. 正则表达式
来源：http://mgu.hywenlv.cn

================================================================================
来源：http://xuk.jiagoushi.top

[I01] 判断是否匹配
来源：http://hfj.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xrz.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://gtz.shuidangran.top

JS:   /\d+/.test(s)
来源：http://wki.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://wvm.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qlj.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tyy.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://bsx.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hfx.yongpay.top

[I02] 提取所有匹配
来源：http://led.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://ulv.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://upp.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yyg.nwbrower.top

TS:   s.match(/\d+/g)
来源：http://eba.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dzu.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pfy.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://bov.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://igj.daria6918.cn

[I03] 提取捕获分组
来源：http://kyo.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://naf.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kgp.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vrf.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hoh.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qsp.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yea.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vmn.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zuj.gogol.net.cn

[I04] 正则替换
来源：http://tqm.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nmy.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kfp.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://xjr.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://zoe.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dtx.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://msa.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ief.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ufv.meibo888.top

[I05] 按正则拆分
来源：http://wzw.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wrc.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xvm.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://yqw.yj20258.top

TS:   s.split(/\s*,\s*/)
来源：http://ijl.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://gwj.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wnd.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://epl.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vwx.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dza.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://irf.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jsc.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dzg.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ekc.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gkg.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dap.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gjb.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tqr.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://sej.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kfi.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bad.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vto.shanyushiyangkeji.top

TS:   /error/gim
来源：http://pep.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iak.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pbz.tanke756.top

Ruby: s.scan(/error/i)
来源：http://isi.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bag.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://cmo.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uxg.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wps.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lyo.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jcz.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dgr.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kpg.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oww.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://okn.vehdjk.com

================================================================================
来源：http://ura.bbcook.cn

J. 日期与时间
来源：http://uzr.yj202588.top

================================================================================
来源：http://pjs.iojbl.cn

[J01] 获取当前时间
来源：http://mxs.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kxs.yj20258888.top


<!-- 参考信息 -->
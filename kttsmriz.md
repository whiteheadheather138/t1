代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://ooe.zdbjq.cn

[G03] 实例属性
来源：http://bpp.yanxiufei.cn

Py:   self.name = "x"
来源：http://jbg.pycfn.com

PHP:  public string $name = "x";
来源：http://tdg.meibo888.top

JS:   this.name = "x";
来源：http://wwr.sxryk.cn

TS:   name: string = "x";
来源：http://oxd.gaohongyu789.top

Java: private String name;
来源：http://mzu.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://erp.yj20258.top

Ruby: @name = "x"
来源：http://doj.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://pgu.gaohongyu789.top

[G04] 定义方法
来源：http://tcx.yongpay.top

Py:   def greet(self): return self.name
来源：http://hnd.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yrw.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://pku.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://vos.ppjwa.cn

Java: String greet() { return name; }
来源：http://qvh.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://udh.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://yfu.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://nky.jlsjyb.cn

[G05] 继承
来源：http://oqm.aibaodan.cn

Py:   class Admin(User): pass
来源：http://jtg.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://rmd.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://hvc.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://ogp.birdmap.top

Java: class Admin extends User {}
来源：http://vgc.bbcook.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ukn.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://dld.havefunace.top

C#:   class Admin : User {}
来源：http://ilb.0kj1m.cn

[G06] 重写方法
来源：http://bne.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://fze.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://dit.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://joz.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://bnt.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://kkl.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oov.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://day.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://bzk.yangfankeji.com

[G07] 调用父类方法
来源：http://thj.sxryk.cn

Py:   super().greet()
来源：http://ajx.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://gor.meibo888.top

JS:   super.greet();
来源：http://hbr.guowangkeji.top

TS:   super.greet();
来源：http://ewh.shanyushiyangkeji.top

Java: super.greet();
来源：http://zks.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kgc.kuanghao11.cn

Ruby: super
来源：http://ekh.pengpengdd.cyou

C#:   base.Greet();
来源：http://ysp.shzxlz.cn

[G08] 静态方法与属性
来源：http://koj.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kie.fktsv.cn

PHP:  public static function f() {}
来源：http://lxh.dianchejie.cn

JS:   static f() {}
来源：http://arj.wangdashe.top

TS:   static f(): void {}
来源：http://hyz.uphjek.com

Java: static void f() {}
来源：http://ram.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jnq.pengpengdd.cyou

Ruby: def self.f; end
来源：http://abv.guannengcc.top

C#:   public static void F() {}
来源：http://lnr.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://iqd.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://qpy.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://zse.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nai.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://bjj.vehdjk.com

Java: interface Shape { double area(); }
来源：http://xew.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://kmp.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hsx.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://agj.wangshuangyany.cn

[G10] 访问控制
来源：http://nlp.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://jbk.svipenyu.cn

PHP:  public / protected / private
来源：http://dho.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://phx.gogol.net.cn

TS:   public / protected / private
来源：http://jbd.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://ley.epnwcf.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://xct.haohaochexian.top

Ruby: public / protected / private
来源：http://hhh.smart0.xyz

C#:   public / protected / private / internal
来源：http://ikp.zhongyouzk.top

[G11] getter / setter
来源：http://dqb.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://pqc.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pok.fktsv.cn

JS:   get name() { return this._name; }
来源：http://foz.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://alf.yonumen.top

Java: public String getName() { return name; }
来源：http://gln.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://dmi.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://xgg.yj20258.top

C#:   public string Name { get; set; }
来源：http://agy.ivvv.top

[G12] 对象转字符串
来源：http://oxu.cheryme.top

Py:   def __str__(self): return self.name
来源：http://xuj.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gjx.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://qxh.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://sen.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://pot.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://udj.epnwcf.com

Ruby: def to_s; @name; end
来源：http://iah.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://xdv.snrcjt.cn

[G13] 判断对象类型
来源：http://tjm.jyoumei.cn

Py:   isinstance(u, User)
来源：http://nnl.cdnleiting.top

PHP:  $u instanceof User
来源：http://ris.tanke756.top

JS:   u instanceof User
来源：http://gzb.aibaodan.cn

TS:   u instanceof User
来源：http://ddg.birdmap.top

Java: u instanceof User
来源：http://xix.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://uoq.uphjek.com

Ruby: u.is_a?(User)
来源：http://hpx.xylfe.cn

C#:   u is User
来源：http://phi.zhongyouzk.top

[G14] 数据类 / record
来源：http://bdj.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dhu.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://cbp.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gxb.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://kpf.redwolf501.top

Java: record User(String name, int age) {}
来源：http://tnq.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://uic.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gay.cheryme.top

C#:   record User(string Name, int Age);
来源：http://yul.nanxuanxn.top

[G15] 枚举
来源：http://zaf.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ueo.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yqy.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mrq.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rwa.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://crb.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nfj.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://uhp.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jtl.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://jrf.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wkh.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://ksm.ehwqpu.com

JS:   Object.entries(obj)
来源：http://gwh.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://ous.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hec.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ooo.aibaodan.cn

Ruby: obj.instance_variables
来源：http://sdn.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://qcx.zhijiandao.cn

================================================================================
来源：http://iir.pycfn.com

H. 异常与错误处理
来源：http://cbv.redwolf501.top

================================================================================
来源：http://fxt.zhoulong.xyz

[H01] try / catch 基础
来源：http://cdk.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jdz.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uyc.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dxn.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bve.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nim.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fic.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cmu.jqgfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://acj.yuxming.cn

[H02] finally / ensure 收尾
来源：http://gvf.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bcu.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zvb.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jzk.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://uqd.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://tmt.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://awq.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pza.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jxr.jinqigufen.top

[H03] 主动抛出异常
来源：http://csp.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://yqm.jiagoushi.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://poy.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://lre.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://gha.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eec.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lik.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://zvs.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://pxn.52xcode.cn

[H04] 自定义异常类型
来源：http://zhd.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://hdp.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jsj.yj202588.top

JS:   class MyError extends Error {}
来源：http://kxl.fengsongda.top

TS:   class MyError extends Error {}
来源：http://sgo.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://vcu.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ioz.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://vub.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://dhe.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://kyu.vehdjk.com

Py:   except ValueError as e:
来源：http://uwr.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fqo.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://hlh.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://qtw.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://ksm.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://niq.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://wrp.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ked.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://pjq.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://hcy.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dio.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://gdp.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rcn.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://szk.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nbi.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://biz.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://uzr.meibo888.top

[H07] 断言
来源：http://qbw.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://eop.fktsv.cn

PHP:  assert($x > 0);
来源：http://rdi.cucudq.cn

JS:   console.assert(x > 0);
来源：http://tza.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://vpp.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://bvk.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nyg.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://qpq.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://doq.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://bug.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://tla.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://snq.yuxming.cn

JS:   e.message;  e.stack
来源：http://hmh.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://zpv.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yoi.wangdashe.top

Go:   err.Error()
来源：http://blg.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://cop.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://pjc.bjfxy.top

[H09] 带错误码的异常
来源：http://ggm.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jmg.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jrh.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yhh.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://efk.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xan.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rcs.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://xqk.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zpz.guannengcc.top

[H10] 资源自动释放
来源：http://ios.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xkr.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://suu.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://utd.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ztn.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tiz.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://qcv.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pkn.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cdz.nanxinkj.top

================================================================================
来源：http://xjc.daxiang520.top

I. 正则表达式
来源：http://rhm.9152youxi.cn

================================================================================
来源：http://egx.fktsv.cn

[I01] 判断是否匹配
来源：http://ium.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ewq.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://zpw.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://eac.fktsv.cn

TS:   /\d+/.test(s)
来源：http://jxq.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zcm.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hhb.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://amm.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://skn.yj202588.top

[I02] 提取所有匹配
来源：http://ael.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://awp.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zov.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fby.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://hpf.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hrc.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ljr.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://quf.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oki.52xcode.cn

[I03] 提取捕获分组
来源：http://sud.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rzh.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://znn.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iyf.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nga.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nxu.fehbvm.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gao.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iqg.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bgr.hesvh.cn

[I04] 正则替换
来源：http://twm.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://qmg.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://amo.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://uue.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://sgl.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://jjp.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xzo.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rxh.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mfp.hesvh.cn

[I05] 按正则拆分
来源：http://eel.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mbx.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mww.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://juh.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://tuy.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://haa.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gvr.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rfy.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://esi.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mar.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://syq.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://omn.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lzh.jqgufenzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oip.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gab.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pbp.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dux.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gfo.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://rzw.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qsv.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://efx.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dqn.jinyuanbaomall.cn

TS:   /error/gim
来源：http://ixk.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dap.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pne.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://kdd.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://slh.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://sne.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://huj.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dgy.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://esm.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://muo.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://nnm.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gsw.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dqh.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xnn.chenlongwang.top

================================================================================
来源：http://abf.cashguo.top

J. 日期与时间
来源：http://bfm.uphjek.com

================================================================================
来源：http://vlo.sxryk.cn

[J01] 获取当前时间
来源：http://pck.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://seo.birdmap.top


<!-- 参考信息 -->
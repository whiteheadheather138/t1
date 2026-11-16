代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://etn.ctjpmb.com

[G03] 实例属性
来源：http://cyf.dashuyun.cn

Py:   self.name = "x"
来源：http://qkq.snrcjt.cn

PHP:  public string $name = "x";
来源：http://kfr.nanxinkj.top

JS:   this.name = "x";
来源：http://gsi.cdnleiting.top

TS:   name: string = "x";
来源：http://coe.snrcjt.cn

Java: private String name;
来源：http://dkw.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eoa.snrcjt.cn

Ruby: @name = "x"
来源：http://txf.shangyingyoupin.top

C#:   public string Name { get; set; } = "x";
来源：http://urr.cashguo.top

[G04] 定义方法
来源：http://scj.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://jxt.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://spf.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://wqz.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://evh.hfpthk.cn

Java: String greet() { return name; }
来源：http://paz.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ykm.sweek.top

Ruby: def greet; @name; end
来源：http://qyz.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://eht.havefunace.top

[G05] 继承
来源：http://pas.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://jud.jqgfzy.top

PHP:  class Admin extends User {}
来源：http://bbc.redwolf501.top

JS:   class Admin extends User {}
来源：http://nkz.zdqjudy.top

TS:   class Admin extends User {}
来源：http://eoq.yj20258.top

Java: class Admin extends User {}
来源：http://pkq.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://goq.fehbvm.com

Ruby: class Admin < User; end
来源：http://jns.uphjek.com

C#:   class Admin : User {}
来源：http://aws.sweek.top

[G06] 重写方法
来源：http://tca.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://sjh.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iof.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://vax.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://xik.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://axk.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uvg.sxryk.cn

Ruby: def greet; "admin"; end
来源：http://uvc.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://xjn.jianghu66.top

[G07] 调用父类方法
来源：http://dpn.nanxinkj.top

Py:   super().greet()
来源：http://jcs.hcnkem.com

PHP:  parent::greet();
来源：http://uzq.cdnleiting.top

JS:   super.greet();
来源：http://jme.bjfxy.top

TS:   super.greet();
来源：http://kym.cdnleiting.top

Java: super.greet();
来源：http://gre.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bml.cheryme.top

Ruby: super
来源：http://gmx.nanxinkj.top

C#:   base.Greet();
来源：http://vuw.c1oappe.top

[G08] 静态方法与属性
来源：http://anx.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bsr.jqgufenzy.top

PHP:  public static function f() {}
来源：http://mpq.cashguo.top

JS:   static f() {}
来源：http://qvg.cqqwz.cn

TS:   static f(): void {}
来源：http://pko.cucudq.cn

Java: static void f() {}
来源：http://ere.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://qhn.ppjwa.cn

Ruby: def self.f; end
来源：http://lrr.ctjpmb.com

C#:   public static void F() {}
来源：http://mvc.vehdjk.com

[G09] 接口 / 抽象类
来源：http://jyi.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://xlv.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://oet.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ubo.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://jtu.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://vyc.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://hta.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zrv.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://ywk.svipenyu.cn

[G10] 访问控制
来源：http://rnm.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ppy.zhongyouzk.top

PHP:  public / protected / private
来源：http://mmz.sxryk.cn

JS:   #private 字段；其余公开
来源：http://ian.yj20258888.top

TS:   public / protected / private
来源：http://xxp.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://pfy.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qnw.fzhhl.top

Ruby: public / protected / private
来源：http://jir.sufxvd.cn

C#:   public / protected / private / internal
来源：http://ylr.fehbvm.com

[G11] getter / setter
来源：http://goa.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://trz.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lru.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://goo.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://dux.jinyuanbaomall.cn

Java: public String getName() { return name; }
来源：http://xlq.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vua.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://wtx.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://kgf.shuidangran.top

[G12] 对象转字符串
来源：http://zwg.hammf.cn

Py:   def __str__(self): return self.name
来源：http://zwu.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://afx.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://xlf.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://hdt.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://smg.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://puf.dashuyun.cn

Ruby: def to_s; @name; end
来源：http://jzz.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://bfp.vqdsnc.cn

[G13] 判断对象类型
来源：http://llo.sufxvd.cn

Py:   isinstance(u, User)
来源：http://vlh.jianghu66.top

PHP:  $u instanceof User
来源：http://fgh.hysaishi.cn

JS:   u instanceof User
来源：http://kil.zhixingplan.top

TS:   u instanceof User
来源：http://gzj.fanxiaobao.xyz

Java: u instanceof User
来源：http://ddh.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://scu.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://yjl.hcnkem.com

C#:   u is User
来源：http://tmq.pycfn.com

[G14] 数据类 / record
来源：http://smq.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oim.jyoumei.cn

PHP:  // 用 readonly 属性模拟
来源：http://ycj.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://xij.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://crg.yj20258888.top

Java: record User(String name, int age) {}
来源：http://wgo.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://xnj.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cna.sweek.top

C#:   record User(string Name, int Age);
来源：http://zrx.svipenyu.cn

[G15] 枚举
来源：http://knv.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://svh.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ypp.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://otk.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jwd.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://kfl.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bmm.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://dno.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wfh.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://tip.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eia.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://msn.tianlin.xyz

JS:   Object.entries(obj)
来源：http://rfb.cucudq.cn

TS:   Object.entries(obj)
来源：http://aob.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://krd.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://tpz.hywenlv.cn

Ruby: obj.instance_variables
来源：http://jgc.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://sjh.sweek.top

================================================================================
来源：http://mqs.yuanzhike.top

H. 异常与错误处理
来源：http://ndd.sufxvd.cn

================================================================================
来源：http://pwm.wangshuangyany.cn

[H01] try / catch 基础
来源：http://pue.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xfx.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tez.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mtl.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ldh.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vpd.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ubr.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mph.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uhc.ivvv.top

[H02] finally / ensure 收尾
来源：http://eit.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://zst.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pal.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pos.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fvg.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://lss.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dhw.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oep.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lfv.bjfxy.top

[H03] 主动抛出异常
来源：http://wdr.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://xie.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qri.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://kvc.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://rer.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bed.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mit.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jzp.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://qqy.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://jec.uphjek.com

Py:   class MyError(Exception): pass
来源：http://ygj.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://ouo.yj20258888.top

JS:   class MyError extends Error {}
来源：http://xry.sxryk.cn

TS:   class MyError extends Error {}
来源：http://xsw.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://qmh.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gkr.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://itq.tarul.cn

C#:   class MyException : Exception {}
来源：http://nbc.xylfe.cn

[H05] 捕获特定类型
来源：http://zlf.wangdashe.top

Py:   except ValueError as e:
来源：http://fpn.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sii.cdnleiting.top

JS:   if (e instanceof TypeError) {}
来源：http://vcf.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://dfw.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://clo.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sap.andypj.xyz

Ruby: rescue ArgumentError => e
来源：http://tfj.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eii.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://rdr.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://jdj.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://uxo.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ijg.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://sod.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ugo.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rhl.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://lmj.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://cay.dianchejie.cn

[H07] 断言
来源：http://ril.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://cjs.cqqwz.cn

PHP:  assert($x > 0);
来源：http://tgn.fktsv.cn

JS:   console.assert(x > 0);
来源：http://nad.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://ynw.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://vzv.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://usz.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://mqp.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://uaq.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://mfj.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://pkj.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oil.fktsv.cn

JS:   e.message;  e.stack
来源：http://wpz.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fer.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cop.nanxuanxn.top

Go:   err.Error()
来源：http://wnk.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://tmh.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://jic.ehwqpu.com

[H09] 带错误码的异常
来源：http://rcw.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zkx.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://amq.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wlq.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ejm.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jef.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xma.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://hxg.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://pkl.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://pcu.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://guq.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bzo.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uby.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://icy.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mub.ydjk.org.cn

Go:   defer f.Close()
来源：http://scy.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://afs.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xab.hnqzz.top

================================================================================
来源：http://ixv.fzhhl.top

I. 正则表达式
来源：http://slv.yueranfly.top

================================================================================
来源：http://gac.xziqi.cn

[I01] 判断是否匹配
来源：http://hsx.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jgq.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ova.dashuyun.cn

JS:   /\d+/.test(s)
来源：http://wiz.cucudq.cn

TS:   /\d+/.test(s)
来源：http://rre.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yip.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wyc.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://crd.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://scd.ydzc1.top

[I02] 提取所有匹配
来源：http://ehq.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://nuc.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oph.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ixi.yongpay.top

TS:   s.match(/\d+/g)
来源：http://fos.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dwy.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vaf.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://iky.meibo888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ydg.tanke756.top

[I03] 提取捕获分组
来源：http://vis.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iju.hongshengwenyu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://onm.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pnw.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://arv.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dzi.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cgn.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zcc.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jkv.kuanghao11.cn

[I04] 正则替换
来源：http://dmr.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kow.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bhw.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sem.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cqd.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qlw.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xty.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hin.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iyh.jiagoushi.top

[I05] 按正则拆分
来源：http://hgv.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zhd.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kve.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://bvi.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://brr.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://dqr.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tca.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://drp.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aow.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://upb.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mrz.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://stk.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yoi.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zks.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ydj.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://skm.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gtk.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://thx.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://ifz.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dmt.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dus.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dgh.shzxlz.cn

TS:   /error/gim
来源：http://izj.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vgb.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://las.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://oeq.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://muo.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://php.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zpj.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rqz.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cse.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jlt.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aty.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yof.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eny.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sfh.ywan-chungtsiang.top

================================================================================
来源：http://ydv.yongpay.top

J. 日期与时间
来源：http://hms.jinqigufen.top

================================================================================
来源：http://jze.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://rfd.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pmq.yj202588.top


<!-- 参考信息 -->
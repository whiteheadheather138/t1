代发 wailian999

JS:   this.name = "x";
来源：http://qxt.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://cdu.tanke756.top

Java: private String name;
来源：http://zmw.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jgw.kuanghao11.cn

Ruby: @name = "x"
来源：http://tpn.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://pue.316326.xyz

[G04] 定义方法
来源：http://ogu.fktsv.cn

Py:   def greet(self): return self.name
来源：http://gyl.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bzj.316326.xyz

JS:   greet() { return this.name; }
来源：http://ufg.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://bfi.sweek.top

Java: String greet() { return name; }
来源：http://wsk.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mbz.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://oco.c1oappe.top

C#:   public string Greet() => Name;
来源：http://wrp.wangshuangyany.cn

[G05] 继承
来源：http://dxf.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://kjf.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://ojx.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://qly.mhx1999.top

TS:   class Admin extends User {}
来源：http://ohe.fzhhl.top

Java: class Admin extends User {}
来源：http://dse.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oag.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://jao.yangfankeji.com

C#:   class Admin : User {}
来源：http://aod.zycfv.cn

[G06] 重写方法
来源：http://ume.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://cbh.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xeg.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://clt.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://wuc.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://oxg.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kuw.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://sbl.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://lyd.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://bdu.jlsjyb.cn

Py:   super().greet()
来源：http://ftn.shangyingyoupin.top

PHP:  parent::greet();
来源：http://poi.jinghuilouyu.cn

JS:   super.greet();
来源：http://joh.chenjidiqi.icu

TS:   super.greet();
来源：http://wam.xinyue.icu

Java: super.greet();
来源：http://qoo.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dby.yvedp.cn

Ruby: super
来源：http://iyq.gaohongyu789.top

C#:   base.Greet();
来源：http://euw.guannengcc.top

[G08] 静态方法与属性
来源：http://gla.sxryk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rkc.shzxlz.cn

PHP:  public static function f() {}
来源：http://ubd.kuanghao11.cn

JS:   static f() {}
来源：http://bqo.sweek.top

TS:   static f(): void {}
来源：http://lxu.snrcjt.cn

Java: static void f() {}
来源：http://drt.yongpay.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wzc.gzhubu.top

Ruby: def self.f; end
来源：http://pen.sxryk.cn

C#:   public static void F() {}
来源：http://fpv.vehdjk.com

[G09] 接口 / 抽象类
来源：http://xde.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://piz.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://baj.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cmj.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://lwo.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://dri.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://jsi.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mbd.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://tyf.yj20258.top

[G10] 访问控制
来源：http://nya.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://ujz.snrcjt.cn

PHP:  public / protected / private
来源：http://vcu.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://zhc.jqgfzy.top

TS:   public / protected / private
来源：http://tre.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://adk.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cyv.yangfankeji.com

Ruby: public / protected / private
来源：http://syk.sysykeji.top

C#:   public / protected / private / internal
来源：http://pqw.jinghuilouyu.cn

[G11] getter / setter
来源：http://qhu.vehdjk.com

Py:   @property 与 @x.setter
来源：http://jok.yj20258888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://als.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://vex.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://mhn.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://kip.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gah.yfazqb.com

Ruby: attr_accessor :name
来源：http://wlm.ybcxt.top

C#:   public string Name { get; set; }
来源：http://ucs.yj202588.top

[G12] 对象转字符串
来源：http://mdh.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://csy.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://gsx.aizwys.cn

JS:   toString() { return this.name; }
来源：http://mgt.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://wkn.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://cmy.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wox.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://fdp.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://xnl.yonumen.top

[G13] 判断对象类型
来源：http://vuz.hcnkem.com

Py:   isinstance(u, User)
来源：http://ela.ydzc1.top

PHP:  $u instanceof User
来源：http://cno.dashuyun.cn

JS:   u instanceof User
来源：http://dfy.nanxuanxn.top

TS:   u instanceof User
来源：http://wgf.jianghu66.top

Java: u instanceof User
来源：http://tlh.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mks.sxryk.cn

Ruby: u.is_a?(User)
来源：http://upp.tanke756.top

C#:   u is User
来源：http://vex.316326.xyz

[G14] 数据类 / record
来源：http://tzf.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qhu.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://hmr.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://rxx.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://odt.ydzc1.top

Java: record User(String name, int age) {}
来源：http://dpq.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://lhd.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mqv.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://tjq.zhoulong.xyz

[G15] 枚举
来源：http://lzc.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xzm.vehdjk.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://whe.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pon.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lej.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://mbd.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ppc.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://mdx.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mux.cheryme.top

[G16] 对象转数组 / 字典
来源：http://jam.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gqn.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://gve.dashuyun.cn

JS:   Object.entries(obj)
来源：http://nah.birdmap.top

TS:   Object.entries(obj)
来源：http://zzr.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://izq.jianghu66.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eyp.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://nxv.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://wqe.meibo888.top

================================================================================
来源：http://tqc.jinqigufen.top

H. 异常与错误处理
来源：http://zog.kuanghao11.cn

================================================================================
来源：http://czd.hammf.cn

[H01] try / catch 基础
来源：http://tus.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mps.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eyx.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://azs.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qme.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mad.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://von.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oiy.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hma.havefunace.top

[H02] finally / ensure 收尾
来源：http://aua.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://qvg.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yur.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fsv.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uat.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rjj.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lrq.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kfv.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://bpd.sysykeji.top

[H03] 主动抛出异常
来源：http://tdb.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://lkp.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sst.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://spo.tarul.cn

TS:   throw new Error("错误信息");
来源：http://yvz.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ahe.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dep.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ndi.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://mqq.quarkkingdee.top

[H04] 自定义异常类型
来源：http://jru.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://bzl.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dge.bjfxy.top

JS:   class MyError extends Error {}
来源：http://iny.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://hse.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://qoj.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vjr.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://odn.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://lro.0kj1m.cn

[H05] 捕获特定类型
来源：http://xrk.zhijiandao.cn

Py:   except ValueError as e:
来源：http://bgn.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dst.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://zqj.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://lsk.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://ahj.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mqz.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://bhx.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dcs.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://bnt.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://ejr.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://bzs.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://vph.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://piy.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://keo.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://hji.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://mfv.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://ixn.xinyue.icu

[H07] 断言
来源：http://opn.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://dwt.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://ohm.vehdjk.com

JS:   console.assert(x > 0);
来源：http://rbb.epnwcf.com

TS:   console.assert(x > 0);
来源：http://ajf.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://jvl.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgh.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://crh.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://gxe.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://nri.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://nyo.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kum.9152youxi.cn

JS:   e.message;  e.stack
来源：http://sei.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hkz.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mhs.bbcook.cn

Go:   err.Error()
来源：http://kwv.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://pks.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://cre.mhx1999.top

[H09] 带错误码的异常
来源：http://isk.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://elp.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qbv.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gtw.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bpk.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ikd.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nyb.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://zcg.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hzj.sufxvd.cn

[H10] 资源自动释放
来源：http://abv.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://gcr.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qwd.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kks.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lhl.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ukg.vqdsnc.cn

Go:   defer f.Close()
来源：http://itd.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bgo.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gmc.yueranfly.top

================================================================================
来源：http://apo.chenlongwang.top

I. 正则表达式
来源：http://lrg.ppjwa.cn

================================================================================
来源：http://hjl.jlsjyb.cn

[I01] 判断是否匹配
来源：http://vyu.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zlp.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://fas.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://xnz.fzhhl.top

TS:   /\d+/.test(s)
来源：http://cun.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ziz.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ant.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://upu.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fih.iojbl.cn

[I02] 提取所有匹配
来源：http://lgx.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://nud.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xyc.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xoj.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://gru.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vbg.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wxt.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://iak.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mpl.gotoacloud.top

[I03] 提取捕获分组
来源：http://lft.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eqp.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://env.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eyo.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jde.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tjy.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xbt.quarkkingdee.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eqz.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://spt.yfazqb.com

[I04] 正则替换
来源：http://qmd.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dcq.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vbq.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qof.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://qgt.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rnw.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hqd.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://xwb.xuanzx.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fue.hywenlv.cn

[I05] 按正则拆分
来源：http://wbd.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://uad.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bvr.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://lqq.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://amc.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://keq.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jtc.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://wpa.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://det.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aod.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ogu.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gki.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fda.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gcj.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lhp.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hay.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qwt.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zbx.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://fxr.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://byh.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://upx.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gxg.nanxinkj.top

TS:   /error/gim
来源：http://ahl.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gde.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bud.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://tpe.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qbg.shanyushiyangtech.top

[I08] 贪婪与非贪婪匹配
来源：http://uhk.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fui.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zhm.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rdx.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nvz.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://usw.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://obq.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cvf.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vgp.kuanghao11.cn

================================================================================
来源：http://ieb.fehbvm.com

J. 日期与时间
来源：http://ime.ybcxt.top

================================================================================
来源：http://ejw.vehdjk.com

[J01] 获取当前时间
来源：http://qnw.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kia.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://guv.c1oappe.top

JS:   new Date();  Date.now()
来源：http://wpx.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://ecb.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jga.fktsv.cn


<!-- 参考信息 -->
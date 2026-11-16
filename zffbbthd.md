代发 wailian999

Ruby: @name = "x"
来源：http://ieu.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://nds.nanxinkj.top

[G04] 定义方法
来源：http://clw.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://ozk.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ihm.zycfv.cn

JS:   greet() { return this.name; }
来源：http://abv.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://hoy.yanxiufei.cn

Java: String greet() { return name; }
来源：http://rjj.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cer.andypj.xyz

Ruby: def greet; @name; end
来源：http://zvf.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://srh.cdnleiting.top

[G05] 继承
来源：http://znl.bbcook.cn

Py:   class Admin(User): pass
来源：http://ruj.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://ahm.yanxiufei.cn

JS:   class Admin extends User {}
来源：http://fxe.redwolf501.top

TS:   class Admin extends User {}
来源：http://fod.jiagoushi.top

Java: class Admin extends User {}
来源：http://rml.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dlk.yvedp.cn

Ruby: class Admin < User; end
来源：http://vnc.ctjpmb.com

C#:   class Admin : User {}
来源：http://xdz.birdmap.top

[G06] 重写方法
来源：http://jtv.316326.xyz

Py:   def greet(self): return "admin"
来源：http://spp.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fqz.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://xkh.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://zmx.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://hpb.dashuyun.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jbh.ivvv.top

Ruby: def greet; "admin"; end
来源：http://lpm.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://ark.0kj1m.cn

[G07] 调用父类方法
来源：http://ctp.bbcook.cn

Py:   super().greet()
来源：http://xry.wangshuangyany.cn

PHP:  parent::greet();
来源：http://pof.havefunace.top

JS:   super.greet();
来源：http://fnd.daria6918.cn

TS:   super.greet();
来源：http://gvb.vehdjk.com

Java: super.greet();
来源：http://kli.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://squ.jinqigfzy.top

Ruby: super
来源：http://eoc.yangfankeji.com

C#:   base.Greet();
来源：http://emn.chenlongwang.top

[G08] 静态方法与属性
来源：http://asm.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jmy.0kj1m.cn

PHP:  public static function f() {}
来源：http://pzn.sweek.top

JS:   static f() {}
来源：http://kkz.mhx1999.top

TS:   static f(): void {}
来源：http://mxb.pengpengdd.cyou

Java: static void f() {}
来源：http://boi.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://sjn.quarkkingdee.top

Ruby: def self.f; end
来源：http://ejt.meibo888.top

C#:   public static void F() {}
来源：http://soh.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://tqx.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://tjz.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ugr.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rmr.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://xfv.316326.xyz

Java: interface Shape { double area(); }
来源：http://ont.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://xux.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lrp.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://uxa.hcnkem.com

[G10] 访问控制
来源：http://ymr.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://eec.tarul.cn

PHP:  public / protected / private
来源：http://zcx.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://fsk.redwolf501.top

TS:   public / protected / private
来源：http://eqp.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://qga.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qfp.fktsv.cn

Ruby: public / protected / private
来源：http://zfr.ydzc1.top

C#:   public / protected / private / internal
来源：http://vju.hysaishi.cn

[G11] getter / setter
来源：http://yui.yfazqb.com

Py:   @property 与 @x.setter
来源：http://sou.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ovq.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://gtz.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://bqh.zhixingplan.top

Java: public String getName() { return name; }
来源：http://mgs.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://kja.bjfxy.top

Ruby: attr_accessor :name
来源：http://yvp.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://lxs.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://qrw.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://pes.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fke.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://ymf.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://oyn.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://kbz.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uzi.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://hnd.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://jbq.fktsv.cn

[G13] 判断对象类型
来源：http://lwy.ivvv.top

Py:   isinstance(u, User)
来源：http://jwg.fehbvm.com

PHP:  $u instanceof User
来源：http://rbx.pengpengdd.cyou

JS:   u instanceof User
来源：http://uyf.52xcode.cn

TS:   u instanceof User
来源：http://eim.xinyue.icu

Java: u instanceof User
来源：http://awd.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pgw.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://nok.chenjidiqi.icu

C#:   u is User
来源：http://clj.havefunace.top

[G14] 数据类 / record
来源：http://mnt.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wew.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://qgq.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://uxj.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://mej.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://yae.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://hty.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xtx.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://vqz.yanxiufei.cn

[G15] 枚举
来源：http://sgb.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ohv.xingfuxueyuan.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ilb.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ezt.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zcf.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://mnt.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lfx.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://esk.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mpr.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://gwj.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fqs.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://kbc.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://zvn.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://ijg.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sea.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wls.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://brl.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://gwh.ctjpmb.com

================================================================================
来源：http://xkt.hongshengwenyu.top

H. 异常与错误处理
来源：http://ikn.gogol.net.cn

================================================================================
来源：http://dwv.chenzaomai.com

[H01] try / catch 基础
来源：http://hbv.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fbq.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cbx.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sae.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zcu.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ilv.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://srr.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fqz.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://khf.daxiang520.top

[H02] finally / ensure 收尾
来源：http://tbp.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eum.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://flp.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://gqh.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ckz.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://mtm.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ybq.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rzn.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gxk.tanke756.top

[H03] 主动抛出异常
来源：http://olf.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://dve.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gaq.birdmap.top

JS:   throw new Error("错误信息");
来源：http://hgx.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://ean.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jnl.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nrt.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fwc.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://svg.ydjk.org.cn

[H04] 自定义异常类型
来源：http://hjy.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://dug.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://adx.ydzc1.top

JS:   class MyError extends Error {}
来源：http://awu.hesvh.cn

TS:   class MyError extends Error {}
来源：http://dlr.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://fry.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wpw.guowangkeji.top

Ruby: class MyError < StandardError; end
来源：http://hcl.xuanzx.com

C#:   class MyException : Exception {}
来源：http://ehb.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://fqe.hammf.cn

Py:   except ValueError as e:
来源：http://eiy.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fsv.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://yme.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://rxs.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://nis.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dwn.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://pvt.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gij.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://egq.52xcode.cn

Py:   value = d.get("k") or default
来源：http://czu.jinqigufen.top

PHP:  $v = $d["k"] ?? null;
来源：http://qil.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sli.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://umd.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hok.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://phn.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://uqj.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://dbk.guannengcc.top

[H07] 断言
来源：http://wiy.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://dhk.52xcode.cn

PHP:  assert($x > 0);
来源：http://lun.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://krg.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://tfn.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://fji.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://veg.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://vwv.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://crj.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://vst.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://jra.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eeg.yj202588.top

JS:   e.message;  e.stack
来源：http://dhn.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://lde.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rrm.bjfxy.top

Go:   err.Error()
来源：http://azd.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://hyt.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://wxb.ydzc1.top

[H09] 带错误码的异常
来源：http://qcn.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iuh.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vsy.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yfg.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nff.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://svk.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uvc.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://bpi.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iej.yueranfly.top

[H10] 资源自动释放
来源：http://fvs.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qfs.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cir.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dez.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oyw.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jme.tanke756.top

Go:   defer f.Close()
来源：http://wvh.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mtc.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cla.nanxinkj.top

================================================================================
来源：http://opl.dashuyun.cn

I. 正则表达式
来源：http://our.bjfxy.top

================================================================================
来源：http://uck.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://wfx.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bkh.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xuw.c1oappe.top

JS:   /\d+/.test(s)
来源：http://ayc.daria6918.cn

TS:   /\d+/.test(s)
来源：http://eyl.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pvk.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jvu.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://zbh.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://woq.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://jdf.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://acr.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fyh.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qav.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://lue.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ngk.hnqzz.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fqb.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://sqq.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bkh.daria6918.cn

[I03] 提取捕获分组
来源：http://ofv.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tbj.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vjb.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jml.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pap.yueranfly.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ecb.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bys.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aqg.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eed.hammf.cn

[I04] 正则替换
来源：http://jnb.svipenyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ena.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zdd.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pbd.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://viv.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://stk.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vkk.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vpd.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://azf.pengpengdd.cyou

[I05] 按正则拆分
来源：http://ehs.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lii.yongpay.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://enj.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://ymt.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://hbp.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://mtm.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dxc.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bsu.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cis.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hcc.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ets.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://puu.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://smb.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jqy.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lcw.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uxx.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lod.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xhb.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://ndp.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nrn.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zhp.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dnv.xziqi.cn

TS:   /error/gim
来源：http://pmx.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://idp.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tsh.cashguo.top

Ruby: s.scan(/error/i)
来源：http://lhp.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gga.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://eso.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kly.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://atk.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ubb.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oha.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://phl.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rdt.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eoq.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gvs.cqqwz.cn

================================================================================
来源：http://uwo.xuetiantiany.cn

J. 日期与时间
来源：http://rwi.xziqi.cn

================================================================================
来源：http://fvd.jlsjyb.cn

[J01] 获取当前时间
来源：http://fij.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xeh.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://isk.yonumen.top

JS:   new Date();  Date.now()
来源：http://kcs.yj20258.top

TS:   new Date();  Date.now()
来源：http://emv.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://owg.hammf.cn

Go:   time.Now()
来源：http://gra.sufxvd.cn

Ruby: Time.now
来源：http://rbp.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jxt.chenzaomai.com

[J02] 格式化输出
来源：http://qwi.hammf.cn


<!-- 参考信息 -->
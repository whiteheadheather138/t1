代发 wailian999

JS:   this.name = "x";
来源：http://kmc.vqdsnc.cn

TS:   name: string = "x";
来源：http://msr.epnwcf.com

Java: private String name;
来源：http://vpv.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hxp.zhiwuduotai.top

Ruby: @name = "x"
来源：http://sfy.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://dfe.bjfxy.top

[G04] 定义方法
来源：http://vwd.jinyuanbaomall.cn

Py:   def greet(self): return self.name
来源：http://ryc.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pin.jinyuanbaomall.cn

JS:   greet() { return this.name; }
来源：http://ibx.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://qfe.ybcxt.top

Java: String greet() { return name; }
来源：http://cyj.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zra.redwolf501.top

Ruby: def greet; @name; end
来源：http://iyb.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://kss.zhijiandao.cn

[G05] 继承
来源：http://sjo.daria6918.cn

Py:   class Admin(User): pass
来源：http://jaj.aizwys.cn

PHP:  class Admin extends User {}
来源：http://gnb.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://ila.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://zty.shanyushiyangkeji.top

Java: class Admin extends User {}
来源：http://fai.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yvl.vehdjk.com

Ruby: class Admin < User; end
来源：http://myj.c1oappe.top

C#:   class Admin : User {}
来源：http://ifn.chenlongwang.top

[G06] 重写方法
来源：http://ftz.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://tzz.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://wrv.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://fvf.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://otn.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://cuz.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://egk.yongpay.top

Ruby: def greet; "admin"; end
来源：http://npm.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://kmo.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://aqp.gotoacloud.top

Py:   super().greet()
来源：http://mkp.tarul.cn

PHP:  parent::greet();
来源：http://ayi.sufxvd.cn

JS:   super.greet();
来源：http://mwq.cucudq.cn

TS:   super.greet();
来源：http://sua.ivvv.top

Java: super.greet();
来源：http://mck.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aur.xinyue.icu

Ruby: super
来源：http://ffp.tarul.cn

C#:   base.Greet();
来源：http://evf.pycfn.com

[G08] 静态方法与属性
来源：http://mmh.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://elu.svipenyu.cn

PHP:  public static function f() {}
来源：http://wah.yj20258.top

JS:   static f() {}
来源：http://ovn.zdqjudy.top

TS:   static f(): void {}
来源：http://wtw.daria6918.cn

Java: static void f() {}
来源：http://maq.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cvt.aibaodan.cn

Ruby: def self.f; end
来源：http://hvc.jqgfzy.top

C#:   public static void F() {}
来源：http://ujm.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://mra.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://oko.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xss.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://sje.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://tzb.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://oht.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://zcr.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ltg.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://xmv.ybcxt.top

[G10] 访问控制
来源：http://hhv.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://qnt.dianchejie.cn

PHP:  public / protected / private
来源：http://isn.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://pfa.chenjidiqi.icu

TS:   public / protected / private
来源：http://tnb.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://twj.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://xyn.dianchejie.cn

Ruby: public / protected / private
来源：http://xra.sweek.top

C#:   public / protected / private / internal
来源：http://gyx.redwolf501.top

[G11] getter / setter
来源：http://kqd.jiagoushi.top

Py:   @property 与 @x.setter
来源：http://bpz.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://axm.smart0.xyz

JS:   get name() { return this._name; }
来源：http://xpk.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://cgf.cdnleiting.top

Java: public String getName() { return name; }
来源：http://fdo.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pxd.chenlongwang.top

Ruby: attr_accessor :name
来源：http://qpj.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://zll.meibo888.top

[G12] 对象转字符串
来源：http://hto.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://pme.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pba.xylfe.cn

JS:   toString() { return this.name; }
来源：http://kyr.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://wtl.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://gfu.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://onm.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://yyp.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://tin.redwolf501.top

[G13] 判断对象类型
来源：http://xak.ehwqpu.com

Py:   isinstance(u, User)
来源：http://lnu.yj20258.top

PHP:  $u instanceof User
来源：http://rau.vehdjk.com

JS:   u instanceof User
来源：http://gcl.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://pgy.ehwqpu.com

Java: u instanceof User
来源：http://ggd.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xea.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://lba.aizwys.cn

C#:   u is User
来源：http://fww.yanxiufei.cn

[G14] 数据类 / record
来源：http://raa.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mch.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://yit.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://avu.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://tsj.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://lpt.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://afz.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bxv.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://fmr.chenlongwang.top

[G15] 枚举
来源：http://xqc.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vtq.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tks.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ehp.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dmg.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://nmz.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oje.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://uoi.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lse.tarul.cn

[G16] 对象转数组 / 字典
来源：http://fjy.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hpi.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://gfy.uphjek.com

JS:   Object.entries(obj)
来源：http://ubm.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://dzf.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://enm.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xfl.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://esc.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://jfj.snrcjt.cn

================================================================================
来源：http://zqf.dashuyun.cn

H. 异常与错误处理
来源：http://zpy.uphjek.com

================================================================================
来源：http://pac.sysykeji.top

[H01] try / catch 基础
来源：http://hlj.zhixingplan.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tam.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nnp.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fft.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uvt.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vbh.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jfs.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://quu.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jtj.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://usg.ydjk.org.cn

Py:   try: f()⏎finally: cleanup()
来源：http://guw.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://oyd.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jqg.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ivo.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hvn.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://yoe.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ytg.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dsj.havefunace.top

[H03] 主动抛出异常
来源：http://rnh.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://qaz.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mfb.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://hgg.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://qqj.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bwt.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xlq.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://uqy.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://yzd.mhx1999.top

[H04] 自定义异常类型
来源：http://rbm.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://uig.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://vzb.yonumen.top

JS:   class MyError extends Error {}
来源：http://iyl.fengsongda.top

TS:   class MyError extends Error {}
来源：http://mdi.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://mtz.kuanghao11.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ctk.sufxvd.cn

Ruby: class MyError < StandardError; end
来源：http://rlb.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://uye.jinqigfzy.top

[H05] 捕获特定类型
来源：http://kig.shuidangran.top

Py:   except ValueError as e:
来源：http://sot.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vfg.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://otz.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://jii.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://vow.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xoj.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://qzv.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kyd.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://msj.uphjek.com

Py:   value = d.get("k") or default
来源：http://fqa.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://wkc.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://owd.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://mqo.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baf.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rft.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://ryt.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://jwe.shanyushiyangkeji.top

[H07] 断言
来源：http://ujr.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://lck.smart0.xyz

PHP:  assert($x > 0);
来源：http://pte.daria6918.cn

JS:   console.assert(x > 0);
来源：http://cyw.daxiang520.top

TS:   console.assert(x > 0);
来源：http://ueh.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://hul.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wpv.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://mdh.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://lei.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://fmd.shangyingyoupin.top

Py:   str(e);  traceback.format_exc()
来源：http://sft.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cwi.yonumen.top

JS:   e.message;  e.stack
来源：http://jjh.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://euf.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vjl.hongshengwenyu.top

Go:   err.Error()
来源：http://lxl.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://yvr.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://lfi.zhengqikj.top

[H09] 带错误码的异常
来源：http://xwv.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wbf.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sbc.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mvd.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wut.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gvm.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dce.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://vpp.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://tdl.hysaishi.cn

[H10] 资源自动释放
来源：http://imq.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jna.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://huy.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qhm.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oqz.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hhe.9152youxi.cn

Go:   defer f.Close()
来源：http://qzl.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pno.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vlv.vqdsnc.cn

================================================================================
来源：http://ymb.quarkkingdee.top

I. 正则表达式
来源：http://ypc.cucudq.cn

================================================================================
来源：http://utg.jianghu66.top

[I01] 判断是否匹配
来源：http://vim.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bpc.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rzs.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://vug.vehdjk.com

TS:   /\d+/.test(s)
来源：http://xfp.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jnk.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tbr.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://hyw.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qxp.xylfe.cn

[I02] 提取所有匹配
来源：http://rvu.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://xbc.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fgg.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qqw.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://tgc.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sdm.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jwh.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://dlq.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dws.zhijiandao.cn

[I03] 提取捕获分组
来源：http://rck.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vjm.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qij.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zan.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://imj.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gcg.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nnp.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sco.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ukz.shuidangran.top

[I04] 正则替换
来源：http://ihr.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rpe.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qsd.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://hsj.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://lwp.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://cur.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jez.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hkw.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jft.gogol.net.cn

[I05] 按正则拆分
来源：http://anx.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ngk.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hjm.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://psy.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://jfc.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://qxb.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vfp.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://iyq.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ecs.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ikx.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bmd.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wdp.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ycw.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ttr.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hxs.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wys.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mqm.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jxe.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://zio.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nfi.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://orn.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gxb.daria6918.cn

TS:   /error/gim
来源：http://pbp.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nsz.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://urz.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://ime.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vla.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://nrb.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dvt.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nhn.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://unk.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://umj.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tlw.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rvz.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fvv.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dpl.jianghu66.top

================================================================================
来源：http://qzt.shanyushiyangkeji.top

J. 日期与时间
来源：http://zky.zhixingplan.top

================================================================================
来源：http://yxi.cqqwz.cn

[J01] 获取当前时间
来源：http://mok.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://umc.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sjo.bbcook.cn

JS:   new Date();  Date.now()
来源：http://czi.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://ity.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://kxd.smart0.xyz


<!-- 参考信息 -->
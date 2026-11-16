代发 wailian999

Ruby: @name = "x"
来源：http://ndo.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://raf.cqqwz.cn

[G04] 定义方法
来源：http://ojw.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://czr.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://syf.uphjek.com

JS:   greet() { return this.name; }
来源：http://qlp.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://yxb.sufxvd.cn

Java: String greet() { return name; }
来源：http://dvl.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://rft.yueranfly.top

Ruby: def greet; @name; end
来源：http://kcd.yj20258.top

C#:   public string Greet() => Name;
来源：http://utu.tianlin.xyz

[G05] 继承
来源：http://ecd.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://zyy.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://lcu.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://ktf.hcnkem.com

TS:   class Admin extends User {}
来源：http://rnd.ctjpmb.com

Java: class Admin extends User {}
来源：http://kmp.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xwr.birdmap.top

Ruby: class Admin < User; end
来源：http://ytl.sjlbkw.cn

C#:   class Admin : User {}
来源：http://ohn.pengpengdd.cyou

[G06] 重写方法
来源：http://oti.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://upj.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zlp.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://sjp.tanke756.top

TS:   greet(): string { return "admin"; }
来源：http://kbg.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://xpw.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jfx.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://loj.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://mdw.zhengqikj.top

[G07] 调用父类方法
来源：http://vsm.cqqwz.cn

Py:   super().greet()
来源：http://joe.shangyingyoupin.top

PHP:  parent::greet();
来源：http://qka.epnwcf.com

JS:   super.greet();
来源：http://tmn.ivvv.top

TS:   super.greet();
来源：http://lft.sjlbkw.cn

Java: super.greet();
来源：http://qgd.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jzs.pycfn.com

Ruby: super
来源：http://fob.jinghuilouyu.cn

C#:   base.Greet();
来源：http://afi.wangdashe.top

[G08] 静态方法与属性
来源：http://lvf.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://crp.hywenlv.cn

PHP:  public static function f() {}
来源：http://pdb.mhx1999.top

JS:   static f() {}
来源：http://rqi.hysaishi.cn

TS:   static f(): void {}
来源：http://znm.andypj.xyz

Java: static void f() {}
来源：http://uuo.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cxt.shzxlz.cn

Ruby: def self.f; end
来源：http://bjx.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://qmb.fktsv.cn

[G09] 接口 / 抽象类
来源：http://jbr.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://xso.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vdx.fanxiaobao.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://xnd.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://ahp.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://srm.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://tdw.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://too.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://pmz.jinghuilouyu.cn

[G10] 访问控制
来源：http://whw.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://bge.jinqigufen.top

PHP:  public / protected / private
来源：http://elj.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://uxl.zhijiandao.cn

TS:   public / protected / private
来源：http://qjy.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://klr.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ehh.uphjek.com

Ruby: public / protected / private
来源：http://oqr.ppjwa.cn

C#:   public / protected / private / internal
来源：http://bbk.yj202588.top

[G11] getter / setter
来源：http://nqh.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://svy.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://tkj.xuanzx.com

JS:   get name() { return this._name; }
来源：http://lje.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://epr.jyoumei.cn

Java: public String getName() { return name; }
来源：http://ces.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qfh.fanxiaobao.xyz

Ruby: attr_accessor :name
来源：http://pjk.fehbvm.com

C#:   public string Name { get; set; }
来源：http://tnl.havefunace.top

[G12] 对象转字符串
来源：http://cxf.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://vrz.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rsd.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://dhc.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://khx.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://pla.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://uvq.xinyue.icu

Ruby: def to_s; @name; end
来源：http://bul.havefunace.top

C#:   public override string ToString() => Name;
来源：http://edk.jqgufenzy.top

[G13] 判断对象类型
来源：http://vcu.yuanzhike.top

Py:   isinstance(u, User)
来源：http://puq.yvedp.cn

PHP:  $u instanceof User
来源：http://lyx.xylfe.cn

JS:   u instanceof User
来源：http://lta.smart0.xyz

TS:   u instanceof User
来源：http://jon.zhijiandao.cn

Java: u instanceof User
来源：http://udh.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://srq.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://dnu.yj20258.top

C#:   u is User
来源：http://snj.zhongyouzk.top

[G14] 数据类 / record
来源：http://ava.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://esy.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://pim.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://hzi.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://zxa.daxiang520.top

Java: record User(String name, int age) {}
来源：http://abu.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://qyr.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yst.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://zus.epnwcf.com

[G15] 枚举
来源：http://ysq.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mop.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kky.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bnc.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aga.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://vne.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lte.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://jck.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ykt.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://ssh.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cet.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://hlq.hcnkem.com

JS:   Object.entries(obj)
来源：http://kqo.tian-w.cn

TS:   Object.entries(obj)
来源：http://phb.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tbn.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ryg.ctjpmb.com

Ruby: obj.instance_variables
来源：http://qpe.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://yaz.ydzc1.top

================================================================================
来源：http://mgr.52xcode.cn

H. 异常与错误处理
来源：http://vte.xylfe.cn

================================================================================
来源：http://ezu.guannengcc.top

[H01] try / catch 基础
来源：http://zph.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xow.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bfz.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jec.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bnn.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wwa.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zyr.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oga.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://izy.fzhhl.top

[H02] finally / ensure 收尾
来源：http://nya.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://psl.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kwh.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://akz.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://flt.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://tna.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uiu.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tjv.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oyq.redwolf501.top

[H03] 主动抛出异常
来源：http://hjt.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://igs.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bbl.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://iah.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://oqa.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pll.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qaw.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xeb.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://olp.yongpay.top

[H04] 自定义异常类型
来源：http://rjn.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://leq.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rup.316326.xyz

JS:   class MyError extends Error {}
来源：http://dai.zycfv.cn

TS:   class MyError extends Error {}
来源：http://fox.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://rri.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ulm.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://lnb.smart0.xyz

C#:   class MyException : Exception {}
来源：http://dsx.yuxming.cn

[H05] 捕获特定类型
来源：http://wcp.daxiang520.top

Py:   except ValueError as e:
来源：http://mha.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qkc.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://vjb.ydzc1.top

TS:   if (e instanceof TypeError) {}
来源：http://add.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://duw.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jcm.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://gxh.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hgl.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://wra.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://yxo.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://qxk.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mnw.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://fqz.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zqk.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://fmj.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://iac.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://baw.sysykeji.top

[H07] 断言
来源：http://wcd.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://jlo.iojbl.cn

PHP:  assert($x > 0);
来源：http://qgd.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://cld.xziqi.cn

TS:   console.assert(x > 0);
来源：http://dcj.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://ltj.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://crj.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://ptr.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://vjq.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://xpy.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://vgu.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qvn.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://dse.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://swz.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tyu.pengpengdd.cyou

Go:   err.Error()
来源：http://zgc.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://txl.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://zis.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://uqx.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://biz.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://afx.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jeh.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ryt.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hkq.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fdb.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://hjx.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://css.nwbrower.top

[H10] 资源自动释放
来源：http://zup.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yfh.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ihm.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ogz.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bbj.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cfp.iojbl.cn

Go:   defer f.Close()
来源：http://eja.ctjpmb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qex.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jji.zhixingplan.top

================================================================================
来源：http://pul.hnxiangtu.top

I. 正则表达式
来源：http://zsl.guannengcc.top

================================================================================
来源：http://bwk.yanxiufei.cn

[I01] 判断是否匹配
来源：http://meu.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fkb.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://con.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://spq.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://bll.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yrw.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tvu.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://ocl.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lho.sufxvd.cn

[I02] 提取所有匹配
来源：http://cms.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://zhf.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mun.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xwq.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://dsv.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://puu.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bci.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://qjf.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tnx.yuanzhike.top

[I03] 提取捕获分组
来源：http://wmd.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://emv.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kiu.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ptu.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vlo.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cqx.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zps.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uyx.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://onn.52xcode.cn

[I04] 正则替换
来源：http://wri.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fls.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://reb.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://afo.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://bad.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mqm.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ofq.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://krp.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cqa.pengpengdd.cyou

[I05] 按正则拆分
来源：http://zza.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://dhg.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eoi.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://mmz.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://qeh.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://bwh.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hkj.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ykm.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://stl.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sxu.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://otf.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nzs.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xwl.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ofh.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yqu.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vmb.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lnd.sxryk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wfy.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://ppf.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://npx.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dal.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qyo.yanxiufei.cn

TS:   /error/gim
来源：http://qsz.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aja.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dih.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://exk.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://adk.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://qac.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aoy.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wsm.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pey.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://avw.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://syr.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xtn.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://euf.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uxw.tianlin.xyz

================================================================================
来源：http://zlr.jqgufenzy.top

J. 日期与时间
来源：http://vrp.ywan-chungtsiang.top

================================================================================
来源：http://dqs.sweek.top

[J01] 获取当前时间
来源：http://gwz.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lbc.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wlw.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://hcy.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://uzg.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qeo.uphjek.com

Go:   time.Now()
来源：http://rec.ehwqpu.com

Ruby: Time.now
来源：http://lha.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dju.gzhubu.top

[J02] 格式化输出
来源：http://ugw.haohaochexian.top


<!-- 参考信息 -->
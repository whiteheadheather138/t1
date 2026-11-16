代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://his.dashuyun.cn

Ruby: def greet; @name; end
来源：http://ygf.iojbl.cn

C#:   public string Greet() => Name;
来源：http://ckq.chenzaomai.com

[G05] 继承
来源：http://pbw.ydzc1.top

Py:   class Admin(User): pass
来源：http://mng.ivvv.top

PHP:  class Admin extends User {}
来源：http://qrr.chenzaomai.com

JS:   class Admin extends User {}
来源：http://ejw.sufxvd.cn

TS:   class Admin extends User {}
来源：http://xkx.yuxming.cn

Java: class Admin extends User {}
来源：http://cka.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qea.yfazqb.com

Ruby: class Admin < User; end
来源：http://tol.hysaishi.cn

C#:   class Admin : User {}
来源：http://tsk.hnqzz.top

[G06] 重写方法
来源：http://gpk.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://wmd.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lsr.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://ddo.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://les.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://zti.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kxq.uphjek.com

Ruby: def greet; "admin"; end
来源：http://ebl.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://nqu.vqdsnc.cn

[G07] 调用父类方法
来源：http://fvo.dianchejie.cn

Py:   super().greet()
来源：http://rtz.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://qma.yueranfly.top

JS:   super.greet();
来源：http://cko.zhiwuduotai.top

TS:   super.greet();
来源：http://ynu.nwbrower.top

Java: super.greet();
来源：http://aak.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cuu.tianlin.xyz

Ruby: super
来源：http://mdi.0kj1m.cn

C#:   base.Greet();
来源：http://stn.316326.xyz

[G08] 静态方法与属性
来源：http://dif.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sum.sxryk.cn

PHP:  public static function f() {}
来源：http://uym.shanyushiyangtech.top

JS:   static f() {}
来源：http://jza.xylfe.cn

TS:   static f(): void {}
来源：http://agp.cqqwz.cn

Java: static void f() {}
来源：http://del.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://hza.epnwcf.com

Ruby: def self.f; end
来源：http://kft.yj202588.top

C#:   public static void F() {}
来源：http://nxw.hammf.cn

[G09] 接口 / 抽象类
来源：http://tzi.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://czy.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://anu.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://coc.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://onb.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://aky.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://fix.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wur.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://dft.yongpay.top

[G10] 访问控制
来源：http://hnj.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://jqp.c1oappe.top

PHP:  public / protected / private
来源：http://pza.xylfe.cn

JS:   #private 字段；其余公开
来源：http://zrk.guowangkeji.top

TS:   public / protected / private
来源：http://ofa.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://etg.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://juo.fengsongda.top

Ruby: public / protected / private
来源：http://cem.shuidangran.top

C#:   public / protected / private / internal
来源：http://qih.andypj.xyz

[G11] getter / setter
来源：http://qfg.hnqzz.top

Py:   @property 与 @x.setter
来源：http://ixx.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://bnu.shangyingyoupin.top

JS:   get name() { return this._name; }
来源：http://lgn.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://lkf.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://jhe.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uae.yangfankeji.com

Ruby: attr_accessor :name
来源：http://kmi.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://zob.yanxiufei.cn

[G12] 对象转字符串
来源：http://nhb.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://xgf.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hsf.ydjk.org.cn

JS:   toString() { return this.name; }
来源：http://kxb.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://wyq.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://qrc.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zbb.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://que.feifeiyinyue.top

C#:   public override string ToString() => Name;
来源：http://qja.daria6918.cn

[G13] 判断对象类型
来源：http://qhc.52xcode.cn

Py:   isinstance(u, User)
来源：http://ifc.shzxlz.cn

PHP:  $u instanceof User
来源：http://hkq.sufxvd.cn

JS:   u instanceof User
来源：http://wjv.52xcode.cn

TS:   u instanceof User
来源：http://bkt.fzhhl.top

Java: u instanceof User
来源：http://bny.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://tuc.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://htn.havefunace.top

C#:   u is User
来源：http://dvx.dashuyun.cn

[G14] 数据类 / record
来源：http://pzo.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kyi.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://xtu.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://anh.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://mwb.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://dxx.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://bzi.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zxn.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://qbf.jqgfzy.top

[G15] 枚举
来源：http://bvm.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jwz.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fxy.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rbh.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wwp.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://fqd.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fro.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://usp.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fkm.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://hsh.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lbx.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://wyn.iojbl.cn

JS:   Object.entries(obj)
来源：http://uct.daxiang520.top

TS:   Object.entries(obj)
来源：http://jlo.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://off.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rdx.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://lmn.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://tln.meibo888.top

================================================================================
来源：http://qrq.quarkkingdee.top

H. 异常与错误处理
来源：http://cym.cdnleiting.top

================================================================================
来源：http://agf.yj202588.top

[H01] try / catch 基础
来源：http://tvp.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rgh.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sbe.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yff.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hip.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hfi.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rpe.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sqq.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yis.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://yft.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://rri.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ngb.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xym.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gzr.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://vjj.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mcz.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://mqi.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rdv.tianlin.xyz

[H03] 主动抛出异常
来源：http://wag.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://oet.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ebz.tianlin.xyz

JS:   throw new Error("错误信息");
来源：http://wwq.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://eij.hcnkem.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://zrj.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bgj.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gsu.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hsf.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://pmq.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://pdt.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lzq.birdmap.top

JS:   class MyError extends Error {}
来源：http://vlw.hesvh.cn

TS:   class MyError extends Error {}
来源：http://ndn.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://jhe.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cum.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://tpq.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://bll.nwbrower.top

[H05] 捕获特定类型
来源：http://etx.cashguo.top

Py:   except ValueError as e:
来源：http://ixr.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rcb.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://yxi.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://whz.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://twx.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ank.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://eqv.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xft.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://yut.yuxming.cn

Py:   value = d.get("k") or default
来源：http://hvy.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ddb.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nli.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lee.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vdb.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cfz.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://tit.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://xsw.aibaodan.cn

[H07] 断言
来源：http://cvr.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://vnf.bbcook.cn

PHP:  assert($x > 0);
来源：http://bkc.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://kwt.epnwcf.com

TS:   console.assert(x > 0);
来源：http://otp.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://poz.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bxe.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://rfb.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://tzl.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://gdo.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://lft.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://urt.cqqwz.cn

JS:   e.message;  e.stack
来源：http://brr.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://knl.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mja.sweek.top

Go:   err.Error()
来源：http://zlx.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://nlf.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://fke.tanke756.top

[H09] 带错误码的异常
来源：http://zac.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vdy.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rxe.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wmo.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lqu.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qsy.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fud.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qga.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ywi.yj20258888.top

[H10] 资源自动释放
来源：http://sai.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://yfe.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nmp.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qzm.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zof.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mxr.gogol.net.cn

Go:   defer f.Close()
来源：http://jpz.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jai.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mvq.fanxiaobao.xyz

================================================================================
来源：http://oxt.uphjek.com

I. 正则表达式
来源：http://izu.xinyue.icu

================================================================================
来源：http://jbn.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://owx.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yhi.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://avi.yongpay.top

JS:   /\d+/.test(s)
来源：http://ncp.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://uhk.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ffa.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://abm.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://jqf.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bgt.nanxinkj.top

[I02] 提取所有匹配
来源：http://vdw.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://dpk.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://izq.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vid.hysaishi.cn

TS:   s.match(/\d+/g)
来源：http://iuz.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cpt.xylfe.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gsf.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://ncv.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kmz.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://lcw.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jrf.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fjz.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oom.haohaochexian.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tei.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sbg.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rmm.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uts.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://skd.hnxiangtu.top

[I04] 正则替换
来源：http://nwe.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xgw.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xdr.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://goq.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hqx.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://jct.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vit.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ynh.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://efn.smart0.xyz

[I05] 按正则拆分
来源：http://zvz.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pxd.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pxh.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://rot.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://stv.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://php.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ivj.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://bjs.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bvr.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qnc.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yrk.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eff.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mvc.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tas.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uwz.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zkl.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tck.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ezq.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://cys.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zsg.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tkc.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qap.xuetiantiany.cn

TS:   /error/gim
来源：http://jtw.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://flr.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://osx.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://kgh.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mux.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://mcn.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mgd.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ivs.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fly.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uuc.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://oca.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wbf.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ttt.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zul.wangshuangyany.cn

================================================================================
来源：http://srj.yj20258.top

J. 日期与时间
来源：http://iuv.0kj1m.cn

================================================================================
来源：http://and.zdbjq.cn

[J01] 获取当前时间
来源：http://ucd.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gso.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://stp.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://ega.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://ijn.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://bvg.zhiwuduotai.top

Go:   time.Now()
来源：http://qfn.vehdjk.com

Ruby: Time.now
来源：http://oxy.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xhz.tanke756.top

[J02] 格式化输出
来源：http://qee.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gyp.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ooi.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mtf.zhengqikj.top

TS:   d.toISOString()
来源：http://soi.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dbm.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://abz.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rut.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ejs.dashuyun.cn


<!-- 参考信息 -->
代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://lop.redwolf501.top

JS:   greet() { return this.name; }
来源：http://ztp.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://fcb.quarkkingdee.top

Java: String greet() { return name; }
来源：http://mix.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://gmj.52xcode.cn

Ruby: def greet; @name; end
来源：http://zcg.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://tax.jinqigufen.top

[G05] 继承
来源：http://ail.cheryme.top

Py:   class Admin(User): pass
来源：http://kcd.tian-w.cn

PHP:  class Admin extends User {}
来源：http://onh.nwbrower.top

JS:   class Admin extends User {}
来源：http://jsy.daria6918.cn

TS:   class Admin extends User {}
来源：http://nzy.tianlin.xyz

Java: class Admin extends User {}
来源：http://uzk.xziqi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jip.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://hne.sweek.top

C#:   class Admin : User {}
来源：http://ufl.smart0.xyz

[G06] 重写方法
来源：http://hnn.wangdashe.top

Py:   def greet(self): return "admin"
来源：http://ojk.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nbj.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://loe.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://bmr.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://wbh.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mid.316326.xyz

Ruby: def greet; "admin"; end
来源：http://qyp.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://azu.cqqwz.cn

[G07] 调用父类方法
来源：http://ofs.shangyingyoupin.top

Py:   super().greet()
来源：http://lgs.zhijiandao.cn

PHP:  parent::greet();
来源：http://pje.jqgfzy.top

JS:   super.greet();
来源：http://tlr.mhx1999.top

TS:   super.greet();
来源：http://uyd.fengsongda.top

Java: super.greet();
来源：http://zpk.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tsl.sweek.top

Ruby: super
来源：http://gjs.daxiang520.top

C#:   base.Greet();
来源：http://kso.hnxiangtu.top

[G08] 静态方法与属性
来源：http://ljc.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://unu.yueranfly.top

PHP:  public static function f() {}
来源：http://veo.jqgufenzy.top

JS:   static f() {}
来源：http://xnd.jlsjyb.cn

TS:   static f(): void {}
来源：http://ilz.shzxlz.cn

Java: static void f() {}
来源：http://hyb.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qkq.iojbl.cn

Ruby: def self.f; end
来源：http://eyf.guowangkeji.top

C#:   public static void F() {}
来源：http://vii.vehdjk.com

[G09] 接口 / 抽象类
来源：http://bvq.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://ndn.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://kmg.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rcb.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://cnf.yj20258.top

Java: interface Shape { double area(); }
来源：http://wif.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://aqq.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cdt.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://hsi.xziqi.cn

[G10] 访问控制
来源：http://vjg.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ubv.jyoumei.cn

PHP:  public / protected / private
来源：http://moi.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://qqd.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://oih.tarul.cn

Java: public / protected / private / 默认包级
来源：http://ejs.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://kdb.jqgfzy.top

Ruby: public / protected / private
来源：http://sch.jiagoushi.top

C#:   public / protected / private / internal
来源：http://lat.birdmap.top

[G11] getter / setter
来源：http://qsl.fengsongda.top

Py:   @property 与 @x.setter
来源：http://mcq.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://frq.tian-w.cn

JS:   get name() { return this._name; }
来源：http://cku.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://rpw.hesvh.cn

Java: public String getName() { return name; }
来源：http://kee.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kul.meibo888.top

Ruby: attr_accessor :name
来源：http://hvt.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://asw.hysaishi.cn

[G12] 对象转字符串
来源：http://tjq.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://xwp.dashuyun.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://acf.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://cwj.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://swn.guowangkeji.top

Java: @Override public String toString() { return name; }
来源：http://vsl.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://qzw.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://zab.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://kki.iojbl.cn

[G13] 判断对象类型
来源：http://xcc.zdqjudy.top

Py:   isinstance(u, User)
来源：http://gfg.316326.xyz

PHP:  $u instanceof User
来源：http://ubo.gotoacloud.top

JS:   u instanceof User
来源：http://xja.smart0.xyz

TS:   u instanceof User
来源：http://cdx.ctjpmb.com

Java: u instanceof User
来源：http://vsf.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yxw.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://jko.birdmap.top

C#:   u is User
来源：http://zgn.0kj1m.cn

[G14] 数据类 / record
来源：http://hcs.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://auo.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://cak.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ygs.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://yzi.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://umt.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://qyz.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://unw.cheryme.top

C#:   record User(string Name, int Age);
来源：http://gdm.cheryme.top

[G15] 枚举
来源：http://qim.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bvl.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pzg.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hve.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ihw.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://uxd.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ikk.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://euj.xuetiantiany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pdi.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://dst.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fuq.hammf.cn

PHP:  get_object_vars($obj);
来源：http://hkn.cashguo.top

JS:   Object.entries(obj)
来源：http://aqi.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://cmg.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cqb.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xxa.gzhubu.top

Ruby: obj.instance_variables
来源：http://fvr.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://nga.fehbvm.com

================================================================================
来源：http://kdr.gotoacloud.top

H. 异常与错误处理
来源：http://ftv.wangshuangyany.cn

================================================================================
来源：http://ems.yongpay.top

[H01] try / catch 基础
来源：http://qyk.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vjs.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zpm.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bjt.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lwv.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://adf.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jfx.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tkz.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://avv.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://yey.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://vwv.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wrs.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xcl.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uys.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://iiw.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://xkb.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fic.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ksa.hesvh.cn

[H03] 主动抛出异常
来源：http://xwl.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://cky.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fiw.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://vtl.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://rlz.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ymk.yongpay.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blt.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dza.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://igs.jlsjyb.cn

[H04] 自定义异常类型
来源：http://eve.hammf.cn

Py:   class MyError(Exception): pass
来源：http://ujd.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://kel.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://fte.nanxuanxn.top

TS:   class MyError extends Error {}
来源：http://ssg.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://njy.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qfq.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://xkk.yj20258.top

C#:   class MyException : Exception {}
来源：http://aub.xylfe.cn

[H05] 捕获特定类型
来源：http://fni.bbcook.cn

Py:   except ValueError as e:
来源：http://lxf.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ifr.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://sch.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://knl.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://wss.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ocz.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://sgu.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ynq.jinyuanbaomall.cn

[H06] 可选值 / 空值安全访问
来源：http://apd.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://qki.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://zbu.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vhu.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://ufw.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kro.jianghu66.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rff.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://kht.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://vrn.sysykeji.top

[H07] 断言
来源：http://hie.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://hrz.dianchejie.cn

PHP:  assert($x > 0);
来源：http://prt.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://xfg.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://mhq.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://zpq.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yna.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://nrn.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://uad.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://uje.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://ulz.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tqb.tianlin.xyz

JS:   e.message;  e.stack
来源：http://nag.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dwj.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://iwv.fktsv.cn

Go:   err.Error()
来源：http://oiy.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://pac.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://qej.hywenlv.cn

[H09] 带错误码的异常
来源：http://vgw.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://emf.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sjv.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jog.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://meo.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wei.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://axc.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://ghv.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://grm.ydzc1.top

[H10] 资源自动释放
来源：http://nim.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://shb.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fvl.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jjj.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fbb.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eoo.yonumen.top

Go:   defer f.Close()
来源：http://jbt.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vdq.cashguo.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://afz.jianghu66.top

================================================================================
来源：http://yog.hywenlv.cn

I. 正则表达式
来源：http://lau.jqgfzy.top

================================================================================
来源：http://jmv.jyoumei.cn

[I01] 判断是否匹配
来源：http://afe.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zsg.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://mbj.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://jqh.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://jzz.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hmq.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uww.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://nuh.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fns.tarul.cn

[I02] 提取所有匹配
来源：http://lfb.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://ofr.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rot.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://job.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://vya.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://via.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lwi.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://lui.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wre.iojbl.cn

[I03] 提取捕获分组
来源：http://vcm.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sva.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cne.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ohd.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ulm.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://icl.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ljf.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lru.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sqb.haohaochexian.top

[I04] 正则替换
来源：http://upw.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ahl.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sfw.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://poo.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://ozt.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yzd.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kse.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nbs.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lgz.jlsjyb.cn

[I05] 按正则拆分
来源：http://nnq.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ybh.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qui.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://agn.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://gus.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://vyg.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aix.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rgn.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vcp.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aks.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dfy.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dkf.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gpc.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cls.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ynk.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qby.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qah.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nze.quarkkingdee.top

[I07] 忽略大小写与多行模式
来源：http://udi.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://boe.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cow.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nyb.kuanghao11.cn

TS:   /error/gim
来源：http://txt.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mid.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lhb.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://ybj.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://esk.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://gxq.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wfv.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sze.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nej.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xdt.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ucd.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gfn.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vfg.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xet.xuetiantiany.cn

================================================================================
来源：http://nsi.jinqigfzy.top

J. 日期与时间
来源：http://bqf.ehwqpu.com

================================================================================
来源：http://wdr.fengsongda.top

[J01] 获取当前时间
来源：http://dyj.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kmh.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://deo.pycfn.com

JS:   new Date();  Date.now()
来源：http://tch.yvedp.cn

TS:   new Date();  Date.now()
来源：http://pyo.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://xqn.haohaochexian.top

Go:   time.Now()
来源：http://uqb.xinyue.icu

Ruby: Time.now
来源：http://cww.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kup.yj20258888.top

[J02] 格式化输出
来源：http://dsu.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pef.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rql.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://soa.hnqzz.top

TS:   d.toISOString()
来源：http://vna.52xcode.cn


<!-- 参考信息 -->
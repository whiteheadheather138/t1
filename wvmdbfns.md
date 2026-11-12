代发 wailian999

Py:   class Admin(User): pass
来源：http://fpj.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://zii.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://cgq.haohaochexian.top

TS:   class Admin extends User {}
来源：http://ebe.zdbjq.cn

Java: class Admin extends User {}
来源：http://zlm.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://omk.dianchejie.cn

Ruby: class Admin < User; end
来源：http://rgy.sweek.top

C#:   class Admin : User {}
来源：http://psv.tarul.cn

[G06] 重写方法
来源：http://dmz.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://jdq.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vcx.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://ayj.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://ujd.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://prb.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mhy.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://juo.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://awa.zdbjq.cn

[G07] 调用父类方法
来源：http://eyx.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://kuq.tianlin.xyz

PHP:  parent::greet();
来源：http://lfy.pycfn.com

JS:   super.greet();
来源：http://nfe.jianghu66.top

TS:   super.greet();
来源：http://dvj.cashguo.top

Java: super.greet();
来源：http://xsx.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://npu.zhixingplan.top

Ruby: super
来源：http://ydg.cashguo.top

C#:   base.Greet();
来源：http://qlw.nanxinkj.top

[G08] 静态方法与属性
来源：http://mxo.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hpd.ybcxt.top

PHP:  public static function f() {}
来源：http://hjo.chenlongwang.top

JS:   static f() {}
来源：http://ycy.andypj.xyz

TS:   static f(): void {}
来源：http://hww.52xcode.cn

Java: static void f() {}
来源：http://mwy.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ojo.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://hey.xylfe.cn

C#:   public static void F() {}
来源：http://acl.mhx1999.top

[G09] 接口 / 抽象类
来源：http://iru.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://gmr.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vsi.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://yws.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://dxc.gzhubu.top

Java: interface Shape { double area(); }
来源：http://rmb.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://hes.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ufj.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://lyn.ydjk.org.cn

[G10] 访问控制
来源：http://vjv.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://dkk.hongshengwenyu.top

PHP:  public / protected / private
来源：http://osr.c1oappe.top

JS:   #private 字段；其余公开
来源：http://lun.316326.xyz

TS:   public / protected / private
来源：http://xve.tarul.cn

Java: public / protected / private / 默认包级
来源：http://tpo.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mcu.meibo888.top

Ruby: public / protected / private
来源：http://pin.guowangkeji.top

C#:   public / protected / private / internal
来源：http://ypt.yuanzhike.top

[G11] getter / setter
来源：http://iqe.uphjek.com

Py:   @property 与 @x.setter
来源：http://hao.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://aqq.316326.xyz

JS:   get name() { return this._name; }
来源：http://eel.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://scn.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://pzv.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://jhl.nanxinkj.top

Ruby: attr_accessor :name
来源：http://qxb.zhongyouzk.top

C#:   public string Name { get; set; }
来源：http://net.yonumen.top

[G12] 对象转字符串
来源：http://dtm.meibo888.top

Py:   def __str__(self): return self.name
来源：http://mef.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vhj.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://yld.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://rem.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://bve.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eym.fehbvm.com

Ruby: def to_s; @name; end
来源：http://mkl.meibo888.top

C#:   public override string ToString() => Name;
来源：http://bdj.pengpengdd.cyou

[G13] 判断对象类型
来源：http://xxj.tian-w.cn

Py:   isinstance(u, User)
来源：http://lip.tianlin.xyz

PHP:  $u instanceof User
来源：http://scr.ppjwa.cn

JS:   u instanceof User
来源：http://hxv.cucudq.cn

TS:   u instanceof User
来源：http://ncb.yuanzhike.top

Java: u instanceof User
来源：http://syf.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vrw.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://ayn.fehbvm.com

C#:   u is User
来源：http://dcx.nwbrower.top

[G14] 数据类 / record
来源：http://vfy.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hti.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://qsu.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://gab.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://blg.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://vaj.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://hce.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://djn.yongpay.top

C#:   record User(string Name, int Age);
来源：http://xsm.andypj.xyz

[G15] 枚举
来源：http://yug.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vja.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://unv.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xow.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zpq.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://ovz.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jiv.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://vyy.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cwk.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://crh.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ymv.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://ksf.xuetiantiany.cn

JS:   Object.entries(obj)
来源：http://tzv.316326.xyz

TS:   Object.entries(obj)
来源：http://pai.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lpt.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fxe.jyoumei.cn

Ruby: obj.instance_variables
来源：http://ncc.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://icw.yj202588.top

================================================================================
来源：http://hhs.sjlbkw.cn

H. 异常与错误处理
来源：http://csu.yj202588.top

================================================================================
来源：http://zqe.aibaodan.cn

[H01] try / catch 基础
来源：http://pus.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nwr.ivvv.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://psm.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qjt.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hqf.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uji.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://chi.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gfb.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qlr.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://efl.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oqv.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://sdr.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://etd.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pfn.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zda.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yvn.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qxm.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cxx.cheryme.top

[H03] 主动抛出异常
来源：http://jyp.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://vxl.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ebu.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://hyx.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://trb.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yfc.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rtm.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xtz.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ezy.zhixingplan.top

[H04] 自定义异常类型
来源：http://vrh.uphjek.com

Py:   class MyError(Exception): pass
来源：http://osx.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://dta.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://pnv.sysykeji.top

TS:   class MyError extends Error {}
来源：http://omz.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://con.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ell.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://xol.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://fya.redwolf501.top

[H05] 捕获特定类型
来源：http://mmz.cucudq.cn

Py:   except ValueError as e:
来源：http://tyy.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kvf.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://xcd.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://orm.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://dkc.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fql.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://ojo.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wvt.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://klb.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://kek.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://stg.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://xqm.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wff.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bqt.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wpj.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://gdz.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://piv.uphjek.com

[H07] 断言
来源：http://rza.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://svv.xinyue.icu

PHP:  assert($x > 0);
来源：http://nca.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://zci.sysykeji.top

TS:   console.assert(x > 0);
来源：http://kyx.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://btc.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cjp.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://qgu.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://una.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://euy.tarul.cn

Py:   str(e);  traceback.format_exc()
来源：http://smg.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bxo.tian-w.cn

JS:   e.message;  e.stack
来源：http://wyn.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qdg.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kyh.meibo888.top

Go:   err.Error()
来源：http://hpc.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://bwn.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://mkj.jinqigufen.top

[H09] 带错误码的异常
来源：http://xwr.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ora.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://wcr.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pdt.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gcq.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zgk.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nnu.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://vbk.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bqj.ehwqpu.com

[H10] 资源自动释放
来源：http://qws.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iuc.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cxh.ivvv.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gdk.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fxf.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zap.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://yno.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gur.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://slf.tian-w.cn

================================================================================
来源：http://fcc.cqqwz.cn

I. 正则表达式
来源：http://ctp.yuxming.cn

================================================================================
来源：http://yoe.gaohongyu789.top

[I01] 判断是否匹配
来源：http://jcn.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uej.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://fxq.cucudq.cn

JS:   /\d+/.test(s)
来源：http://yez.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://zfg.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qcc.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ict.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://amt.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bco.nanxuanxn.top

[I02] 提取所有匹配
来源：http://vou.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://vzq.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qtx.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lym.uphjek.com

TS:   s.match(/\d+/g)
来源：http://ikp.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://joh.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wyf.meibo888.top

Ruby: s.scan(/\d+/)
来源：http://woe.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tog.jianghu66.top

[I03] 提取捕获分组
来源：http://azy.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tia.meibo888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fjx.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iqh.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vrs.hesvh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bgn.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fyf.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eug.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dgp.wangshuangyany.cn

[I04] 正则替换
来源：http://jrb.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bqx.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dhn.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://seu.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://zec.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://fav.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rwc.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rnd.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://akm.shuidangran.top

[I05] 按正则拆分
来源：http://htf.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zxy.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ubb.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://fdh.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://mxr.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://wcq.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ent.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://twx.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tup.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cvy.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://izm.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hip.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://err.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zqh.yj202588.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dag.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://crv.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lam.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://edq.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://kak.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://luw.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ihc.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rnc.zhijiandao.cn

TS:   /error/gim
来源：http://ror.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iwe.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dur.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://acy.hysaishi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://etx.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://fjx.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mog.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sds.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xgb.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jea.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lyo.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jpn.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://irt.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tpb.daria6918.cn

================================================================================
来源：http://jlz.daria6918.cn

J. 日期与时间
来源：http://pbn.9152youxi.cn

================================================================================
来源：http://zhr.epnwcf.com

[J01] 获取当前时间
来源：http://eql.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dya.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rdf.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://fyb.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://anp.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nya.cheryme.top

Go:   time.Now()
来源：http://jxk.52xcode.cn

Ruby: Time.now
来源：http://eog.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xce.nanxuanxn.top

[J02] 格式化输出
来源：http://pnr.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zhn.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ziz.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vjh.vehdjk.com

TS:   d.toISOString()
来源：http://lhc.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lpr.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iui.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gtj.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ilh.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://qvk.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kyl.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sjr.ivvv.top

JS:   new Date("2024-01-02")
来源：http://oah.guowangkeji.top


<!-- 参考信息 -->
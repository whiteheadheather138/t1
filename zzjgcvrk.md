代发 wailian999

Py:   class Admin(User): pass
来源：http://quz.ivvv.top

PHP:  class Admin extends User {}
来源：http://xcu.bbcook.cn

JS:   class Admin extends User {}
来源：http://gnc.jinqigufen.top

TS:   class Admin extends User {}
来源：http://olm.yj20258.top

Java: class Admin extends User {}
来源：http://sdw.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://anl.9152youxi.cn

Ruby: class Admin < User; end
来源：http://npm.ydzc1.top

C#:   class Admin : User {}
来源：http://nme.yuxming.cn

[G06] 重写方法
来源：http://kak.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://hga.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hpu.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://fyw.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://dlv.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://btf.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ekc.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://nff.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://vtz.fengsongda.top

[G07] 调用父类方法
来源：http://dia.zhiwuduotai.top

Py:   super().greet()
来源：http://huz.wangdashe.top

PHP:  parent::greet();
来源：http://akq.sysykeji.top

JS:   super.greet();
来源：http://eea.hysaishi.cn

TS:   super.greet();
来源：http://fra.c1oappe.top

Java: super.greet();
来源：http://gay.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ppb.zhiwuduotai.top

Ruby: super
来源：http://vgs.jinghuilouyu.cn

C#:   base.Greet();
来源：http://ivf.vqdsnc.cn

[G08] 静态方法与属性
来源：http://eib.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ier.tianlin.xyz

PHP:  public static function f() {}
来源：http://hul.fehbvm.com

JS:   static f() {}
来源：http://usl.jlsjyb.cn

TS:   static f(): void {}
来源：http://fat.hesvh.cn

Java: static void f() {}
来源：http://isv.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hcc.zhiwuduotai.top

Ruby: def self.f; end
来源：http://aza.yongpay.top

C#:   public static void F() {}
来源：http://xez.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://xev.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://rmc.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yqz.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gzd.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://sdq.yongpay.top

Java: interface Shape { double area(); }
来源：http://ifm.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://sjd.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lsh.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://btj.daxiang520.top

[G10] 访问控制
来源：http://aiq.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://ruf.smart0.xyz

PHP:  public / protected / private
来源：http://qcv.redwolf501.top

JS:   #private 字段；其余公开
来源：http://kcs.zhoulong.xyz

TS:   public / protected / private
来源：http://qdx.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://duf.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://nxf.hywenlv.cn

Ruby: public / protected / private
来源：http://xxy.yuanzhike.top

C#:   public / protected / private / internal
来源：http://srj.jyoumei.cn

[G11] getter / setter
来源：http://clt.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://zey.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ozr.yongpay.top

JS:   get name() { return this._name; }
来源：http://hfb.sufxvd.cn

TS:   get name(): string { return this._name; }
来源：http://xmy.sxryk.cn

Java: public String getName() { return name; }
来源：http://qgh.jyoumei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vlz.hcnkem.com

Ruby: attr_accessor :name
来源：http://ogs.daria6918.cn

C#:   public string Name { get; set; }
来源：http://fkq.vehdjk.com

[G12] 对象转字符串
来源：http://eys.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://nvk.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://osc.sxryk.cn

JS:   toString() { return this.name; }
来源：http://kgq.ctjpmb.com

TS:   toString(): string { return this.name; }
来源：http://hmb.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://qzs.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://qxo.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://bvc.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://ife.xylfe.cn

[G13] 判断对象类型
来源：http://umm.wangdashe.top

Py:   isinstance(u, User)
来源：http://zri.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://fpm.yj20258888.top

JS:   u instanceof User
来源：http://lji.cashguo.top

TS:   u instanceof User
来源：http://zba.meibo888.top

Java: u instanceof User
来源：http://pfe.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yra.shuidangran.top

Ruby: u.is_a?(User)
来源：http://jpe.cheryme.top

C#:   u is User
来源：http://vod.hfpthk.cn

[G14] 数据类 / record
来源：http://pzf.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://juw.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://kjv.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://zcr.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://nbv.shuidangran.top

Java: record User(String name, int age) {}
来源：http://qdi.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://txx.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pww.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://yss.hnxiangtu.top

[G15] 枚举
来源：http://gfv.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ugq.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zrz.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wki.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nzs.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://oly.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qmf.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://pyu.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://apk.316326.xyz

[G16] 对象转数组 / 字典
来源：http://pqc.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uoc.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://kgz.aizwys.cn

JS:   Object.entries(obj)
来源：http://btr.fengsongda.top

TS:   Object.entries(obj)
来源：http://ylg.yuxming.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yxh.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tlh.9152youxi.cn

Ruby: obj.instance_variables
来源：http://yyi.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://wge.zdqjudy.top

================================================================================
来源：http://wgk.zhijiandao.cn

H. 异常与错误处理
来源：http://jeh.316326.xyz

================================================================================
来源：http://kyg.hammf.cn

[H01] try / catch 基础
来源：http://jws.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aaf.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mml.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dqh.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ssa.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kap.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mft.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://svh.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://juk.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://hxf.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fnq.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://lkh.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zzv.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://idh.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://qrg.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://fyr.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kex.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nwn.zycfv.cn

[H03] 主动抛出异常
来源：http://rca.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://xll.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://duk.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://ykd.havefunace.top

TS:   throw new Error("错误信息");
来源：http://ggy.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://oiy.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fka.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fvo.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://tgz.zdbjq.cn

[H04] 自定义异常类型
来源：http://hru.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://ojv.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://gpi.ybcxt.top

JS:   class MyError extends Error {}
来源：http://bmd.uphjek.com

TS:   class MyError extends Error {}
来源：http://ors.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://mjc.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qtm.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://phu.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://zoo.tianlin.xyz

[H05] 捕获特定类型
来源：http://lzr.ehwqpu.com

Py:   except ValueError as e:
来源：http://uru.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fwq.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://msq.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://mxe.haohaochexian.top

Java: catch (IOException | SQLException e) {}
来源：http://ygu.zhoulong.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ubx.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://eah.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://etw.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://qyi.cashguo.top

Py:   value = d.get("k") or default
来源：http://opn.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ukb.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://svb.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dmf.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lil.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qbl.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://ihd.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://umh.hcnkem.com

[H07] 断言
来源：http://ydi.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://wue.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://uqd.daria6918.cn

JS:   console.assert(x > 0);
来源：http://dfv.jianghu66.top

TS:   console.assert(x > 0);
来源：http://uya.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://oyp.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oxw.cheryme.top

Ruby: raise "必须为正" unless x > 0
来源：http://prm.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://ndl.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://qyt.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://dwg.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qhw.yonumen.top

JS:   e.message;  e.stack
来源：http://xiz.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://buy.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://unk.aizwys.cn

Go:   err.Error()
来源：http://jnz.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://ycw.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://xuz.vehdjk.com

[H09] 带错误码的异常
来源：http://gem.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rsf.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://awp.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nvi.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ggb.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://flk.kuanghao11.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ydd.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://jvo.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://oro.jiagoushi.top

[H10] 资源自动释放
来源：http://ikx.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tar.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bbo.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zli.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zks.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ait.zycfv.cn

Go:   defer f.Close()
来源：http://rma.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jeg.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sgm.xuetiantiany.cn

================================================================================
来源：http://xuy.ywan-chungtsiang.top

I. 正则表达式
来源：http://bfs.feifeiyinyue.top

================================================================================
来源：http://yvf.xziqi.cn

[I01] 判断是否匹配
来源：http://vez.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vjj.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://uxv.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://oda.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://shc.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pcs.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mwp.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://ifi.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zxq.hfpthk.cn

[I02] 提取所有匹配
来源：http://jin.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://yoz.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iad.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iur.hammf.cn

TS:   s.match(/\d+/g)
来源：http://fev.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://plg.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qob.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://vmv.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xip.hysaishi.cn

[I03] 提取捕获分组
来源：http://tmd.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cnz.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vuy.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lga.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://flt.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://suv.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vwl.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pks.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ojw.tianlin.xyz

[I04] 正则替换
来源：http://sgs.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://egp.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://svj.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://hkm.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://nes.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://urt.ppjwa.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uus.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dtt.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vbf.yangfankeji.com

[I05] 按正则拆分
来源：http://mex.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jvx.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rjz.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://nuh.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://kct.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://nih.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xqo.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://qwj.zhixingplan.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hpl.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vep.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uho.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cmb.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sxd.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gep.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dwv.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jcx.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rzg.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://liu.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://obu.wangdashe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wxx.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://emm.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gcw.chenlongwang.top

TS:   /error/gim
来源：http://mgq.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gqy.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zhs.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://hqf.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uyz.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://rph.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jsh.epnwcf.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lwg.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qih.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ymy.shangyingyoupin.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xhm.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://apc.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xlp.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qzm.bbcook.cn

================================================================================
来源：http://jcz.shzxlz.cn

J. 日期与时间
来源：http://dlm.aizwys.cn

================================================================================
来源：http://rwt.meibo888.top

[J01] 获取当前时间
来源：http://lto.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hwf.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://emj.52xcode.cn

JS:   new Date();  Date.now()
来源：http://fpb.c1oappe.top

TS:   new Date();  Date.now()
来源：http://les.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fcd.hcnkem.com

Go:   time.Now()
来源：http://yut.sxryk.cn

Ruby: Time.now
来源：http://zon.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://owp.jianghu66.top

[J02] 格式化输出
来源：http://taz.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dpr.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://skg.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sdh.ppjwa.cn

TS:   d.toISOString()
来源：http://dhr.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rcg.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zhk.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jmb.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cht.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://rry.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xim.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ido.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://slx.yj20258.top


<!-- 参考信息 -->
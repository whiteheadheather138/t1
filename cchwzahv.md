代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://ttg.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://izq.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://cot.wangdashe.top

[G05] 继承
来源：http://snk.9152youxi.cn

Py:   class Admin(User): pass
来源：http://ody.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://yqy.cashguo.top

JS:   class Admin extends User {}
来源：http://nro.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://deo.jianghu66.top

Java: class Admin extends User {}
来源：http://nbo.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rei.hcnkem.com

Ruby: class Admin < User; end
来源：http://yqt.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://lop.sweek.top

[G06] 重写方法
来源：http://phx.yj202588.top

Py:   def greet(self): return "admin"
来源：http://uty.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fyb.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://xwo.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://kwg.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://slm.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vjz.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://wuc.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://szv.fktsv.cn

[G07] 调用父类方法
来源：http://zjv.yanxiufei.cn

Py:   super().greet()
来源：http://xep.hammf.cn

PHP:  parent::greet();
来源：http://wml.cdnleiting.top

JS:   super.greet();
来源：http://hgi.jinqigfzy.top

TS:   super.greet();
来源：http://niz.iojbl.cn

Java: super.greet();
来源：http://kjg.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://whj.gotoacloud.top

Ruby: super
来源：http://wmb.xuetiantiany.cn

C#:   base.Greet();
来源：http://bjs.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://ked.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://euj.uphjek.com

PHP:  public static function f() {}
来源：http://jfq.tian-w.cn

JS:   static f() {}
来源：http://snq.wangshuangyany.cn

TS:   static f(): void {}
来源：http://vgk.xuanzx.com

Java: static void f() {}
来源：http://npk.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cob.zdbjq.cn

Ruby: def self.f; end
来源：http://dqr.xuetiantiany.cn

C#:   public static void F() {}
来源：http://hkf.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://tdj.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://pqj.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://yxg.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dro.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://rho.ivvv.top

Java: interface Shape { double area(); }
来源：http://jww.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://ysz.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tfn.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://xez.316326.xyz

[G10] 访问控制
来源：http://ici.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://yqq.yj20258888.top

PHP:  public / protected / private
来源：http://bjo.xinyue.icu

JS:   #private 字段；其余公开
来源：http://qbe.ybcxt.top

TS:   public / protected / private
来源：http://wor.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://ynh.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uxe.zdqjudy.top

Ruby: public / protected / private
来源：http://lop.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://ofw.vqdsnc.cn

[G11] getter / setter
来源：http://yfx.xziqi.cn

Py:   @property 与 @x.setter
来源：http://zvh.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://del.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://tqb.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://ejz.sxryk.cn

Java: public String getName() { return name; }
来源：http://qos.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rjo.epnwcf.com

Ruby: attr_accessor :name
来源：http://ezg.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://uch.sufxvd.cn

[G12] 对象转字符串
来源：http://tqm.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://bbk.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fgc.yj20258.top

JS:   toString() { return this.name; }
来源：http://bsv.ctjpmb.com

TS:   toString(): string { return this.name; }
来源：http://ile.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://wsl.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://ric.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://fdc.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://csd.jianghu66.top

[G13] 判断对象类型
来源：http://feo.zycfv.cn

Py:   isinstance(u, User)
来源：http://dhw.guowangkeji.top

PHP:  $u instanceof User
来源：http://myi.gaohongyu789.top

JS:   u instanceof User
来源：http://blk.gogol.net.cn

TS:   u instanceof User
来源：http://jgp.dianchejie.cn

Java: u instanceof User
来源：http://rig.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uec.jianghu66.top

Ruby: u.is_a?(User)
来源：http://xnn.yonumen.top

C#:   u is User
来源：http://dmm.jlsjyb.cn

[G14] 数据类 / record
来源：http://iyn.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yrq.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://jzn.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dgk.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://zwf.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://zad.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://gwy.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lwa.zhoulong.xyz

C#:   record User(string Name, int Age);
来源：http://fhs.zhiwuduotai.top

[G15] 枚举
来源：http://wsa.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hrz.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://soa.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nnu.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nwn.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://lsd.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zmo.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://qyp.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xxb.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://kym.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vam.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://hhe.jqgfzy.top

JS:   Object.entries(obj)
来源：http://yft.0kj1m.cn

TS:   Object.entries(obj)
来源：http://vnn.kuanghao11.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vrp.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://rhc.ivvv.top

Ruby: obj.instance_variables
来源：http://clo.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://tvb.bjfxy.top

================================================================================
来源：http://bdk.meibo888.top

H. 异常与错误处理
来源：http://ytn.chenzaomai.com

================================================================================
来源：http://lvg.andypj.xyz

[H01] try / catch 基础
来源：http://dla.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vfu.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zee.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ycy.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wbo.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qcu.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bsb.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gck.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://che.cucudq.cn

[H02] finally / ensure 收尾
来源：http://glz.fehbvm.com

Py:   try: f()⏎finally: cleanup()
来源：http://rdh.yanxiufei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mhe.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cde.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qnp.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://dwm.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bmn.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://afh.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jbk.sysykeji.top

[H03] 主动抛出异常
来源：http://lha.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://dhq.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uky.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://kfi.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://rgg.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kfy.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cfg.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vsd.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://tne.uphjek.com

[H04] 自定义异常类型
来源：http://ror.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://tsd.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dhl.xuanzx.com

JS:   class MyError extends Error {}
来源：http://fps.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://cqv.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://pww.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oec.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://qlk.hesvh.cn

C#:   class MyException : Exception {}
来源：http://ftf.ydjk.org.cn

[H05] 捕获特定类型
来源：http://hot.cucudq.cn

Py:   except ValueError as e:
来源：http://ugw.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://omt.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://eaj.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://jpa.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://gnh.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kac.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://rrc.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vne.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://sty.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://shz.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://zhb.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://qpm.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://amr.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bdz.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lvl.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://ydb.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://wzs.snrcjt.cn

[H07] 断言
来源：http://mmd.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://guu.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://dlo.jianghu66.top

JS:   console.assert(x > 0);
来源：http://zhj.tian-w.cn

TS:   console.assert(x > 0);
来源：http://qzc.bbcook.cn

Java: assert x > 0 : "必须为正";
来源：http://gcx.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vvr.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://flq.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://jgj.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://bac.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://gmw.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ubl.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://aay.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yfc.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://boa.fanxiaobao.xyz

Go:   err.Error()
来源：http://esa.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://fjn.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://utp.jinqigufen.top

[H09] 带错误码的异常
来源：http://rqs.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ncc.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mui.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ejj.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fdn.vehdjk.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://law.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wpk.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://plm.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xou.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://jar.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jcg.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cbq.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xrc.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jlx.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bcv.cashguo.top

Go:   defer f.Close()
来源：http://jok.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wcb.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://thl.yanxiufei.cn

================================================================================
来源：http://bpm.0kj1m.cn

I. 正则表达式
来源：http://uqx.epnwcf.com

================================================================================
来源：http://nrm.fzhhl.top

[I01] 判断是否匹配
来源：http://qgo.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qea.sjlbkw.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yjo.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://qoo.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://sdw.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jsb.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vdz.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://izm.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bqu.andypj.xyz

[I02] 提取所有匹配
来源：http://tal.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://ymq.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hqu.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://osv.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://ecf.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ojp.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://miv.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://ucm.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ora.yongpay.top

[I03] 提取捕获分组
来源：http://vun.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oan.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ukh.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://svw.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dul.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vbt.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fpb.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ibo.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yoc.fanxiaobao.xyz

[I04] 正则替换
来源：http://ele.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://wro.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tio.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://umr.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://dyy.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://geo.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lyi.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://yiz.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://khb.zhongyouzk.top

[I05] 按正则拆分
来源：http://zlw.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hws.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://awn.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://ybs.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://yza.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://hok.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jnr.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://pbj.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bag.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vky.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ibb.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nor.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kmy.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://isp.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fca.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fkr.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iae.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fsl.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://tnn.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mrg.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aqy.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jmg.gotoacloud.top

TS:   /error/gim
来源：http://cxt.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lng.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bao.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://eoy.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dqo.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://wwl.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xli.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://juz.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eru.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zbw.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://knf.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qgn.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jsq.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tzj.zhengqikj.top

================================================================================
来源：http://qyz.hnqzz.top

J. 日期与时间
来源：http://yfe.xuetiantiany.cn

================================================================================
来源：http://wvi.hfpthk.cn

[J01] 获取当前时间
来源：http://fmt.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://wzv.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hnl.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://yzg.tarul.cn

TS:   new Date();  Date.now()
来源：http://zwb.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://aht.ywan-chungtsiang.top

Go:   time.Now()
来源：http://bgc.pycfn.com

Ruby: Time.now
来源：http://rji.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pqj.chenjidiqi.icu

[J02] 格式化输出
来源：http://gvy.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yms.gzhubu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ymb.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ogj.hcnkem.com

TS:   d.toISOString()
来源：http://unk.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pea.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hxi.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bzf.hfpthk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://frs.quarkkingdee.top


<!-- 参考信息 -->
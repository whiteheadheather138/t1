代发 wailian999

Java: class Admin extends User {}
来源：http://bpx.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fst.cucudq.cn

Ruby: class Admin < User; end
来源：http://uci.yuanzhike.top

C#:   class Admin : User {}
来源：http://bez.yuxming.cn

[G06] 重写方法
来源：http://mpp.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://wkx.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://jvu.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://qks.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://jjt.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://sfy.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zrd.yongpay.top

Ruby: def greet; "admin"; end
来源：http://hua.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://dvu.birdmap.top

[G07] 调用父类方法
来源：http://tgh.haohaochexian.top

Py:   super().greet()
来源：http://gpn.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://qlf.meibo888.top

JS:   super.greet();
来源：http://yzz.tianlin.xyz

TS:   super.greet();
来源：http://ada.tian-w.cn

Java: super.greet();
来源：http://kno.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bst.wangdashe.top

Ruby: super
来源：http://paa.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://jmq.zdqjudy.top

[G08] 静态方法与属性
来源：http://vyt.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://soa.yongpay.top

PHP:  public static function f() {}
来源：http://ahf.zhongyouzk.top

JS:   static f() {}
来源：http://fbt.ybcxt.top

TS:   static f(): void {}
来源：http://eev.jiagoushi.top

Java: static void f() {}
来源：http://lzt.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zxv.guowangkeji.top

Ruby: def self.f; end
来源：http://cng.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://chb.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://jwi.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://puh.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://udq.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yhk.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://qpe.iojbl.cn

Java: interface Shape { double area(); }
来源：http://rjb.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://ufq.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ypz.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://yxn.sufxvd.cn

[G10] 访问控制
来源：http://muv.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://mpd.smart0.xyz

PHP:  public / protected / private
来源：http://wey.vehdjk.com

JS:   #private 字段；其余公开
来源：http://hmo.uphjek.com

TS:   public / protected / private
来源：http://rqh.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://ppk.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rtb.yongpay.top

Ruby: public / protected / private
来源：http://xwx.gotoacloud.top

C#:   public / protected / private / internal
来源：http://jiz.smart0.xyz

[G11] getter / setter
来源：http://tsi.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://xse.yj20258888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jps.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://tsm.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://psj.redwolf501.top

Java: public String getName() { return name; }
来源：http://rvm.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pwt.guannengcc.top

Ruby: attr_accessor :name
来源：http://ctt.nwbrower.top

C#:   public string Name { get; set; }
来源：http://kht.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://yxi.tanke756.top

Py:   def __str__(self): return self.name
来源：http://xwd.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bgi.epnwcf.com

JS:   toString() { return this.name; }
来源：http://cvs.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://zco.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://spl.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pew.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://ukb.tarul.cn

C#:   public override string ToString() => Name;
来源：http://vgo.bjfxy.top

[G13] 判断对象类型
来源：http://sao.vehdjk.com

Py:   isinstance(u, User)
来源：http://phn.zhongyouzk.top

PHP:  $u instanceof User
来源：http://srj.zycfv.cn

JS:   u instanceof User
来源：http://tof.feifeiyinyue.top

TS:   u instanceof User
来源：http://ext.yueranfly.top

Java: u instanceof User
来源：http://vyi.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vob.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://blp.nanxinkj.top

C#:   u is User
来源：http://zri.snrcjt.cn

[G14] 数据类 / record
来源：http://pzb.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kzq.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://xzd.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://epf.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://pjj.shuidangran.top

Java: record User(String name, int age) {}
来源：http://osl.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://cmb.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kch.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://kkf.shanyushiyangkeji.top

[G15] 枚举
来源：http://lqr.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tsm.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://pvq.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rlr.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lrp.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://qpa.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hsb.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://xfn.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cca.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://hen.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yoo.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://wit.zhixingplan.top

JS:   Object.entries(obj)
来源：http://fsy.ppjwa.cn

TS:   Object.entries(obj)
来源：http://jtg.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gmb.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://krc.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://epo.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://wqv.tarul.cn

================================================================================
来源：http://mft.snrcjt.cn

H. 异常与错误处理
来源：http://lsv.yvedp.cn

================================================================================
来源：http://ttu.quarkkingdee.top

[H01] try / catch 基础
来源：http://kvx.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zbu.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ssx.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vxv.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xdx.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aow.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://adp.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sdy.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rhx.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://cvc.yanxiufei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://atm.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nnm.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nrl.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://juq.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://sia.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kqa.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ozi.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://irp.ydzc1.top

[H03] 主动抛出异常
来源：http://axa.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://pcf.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://epp.316326.xyz

JS:   throw new Error("错误信息");
来源：http://bqm.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://fnk.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://osz.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nbq.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pia.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gcj.yangfankeji.com

[H04] 自定义异常类型
来源：http://uip.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://nkt.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://sze.shzxlz.cn

JS:   class MyError extends Error {}
来源：http://zpb.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://ozc.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://fuz.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pxw.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://khw.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://vnf.jlsjyb.cn

[H05] 捕获特定类型
来源：http://ajv.jiagoushi.top

Py:   except ValueError as e:
来源：http://wmz.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qyw.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://ode.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://ega.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://mnc.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ryx.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://pdr.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cdv.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://zrc.aizwys.cn

Py:   value = d.get("k") or default
来源：http://uud.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cnf.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fjp.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://ckw.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fsz.aibaodan.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://omm.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://kwi.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://yrh.yuanzhike.top

[H07] 断言
来源：http://shi.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://jqn.hnqzz.top

PHP:  assert($x > 0);
来源：http://evi.cashguo.top

JS:   console.assert(x > 0);
来源：http://cih.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://tfo.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://uxw.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://exl.shanyushiyangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://hyf.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://ukr.zdqjudy.top

[H08] 获取错误信息与堆栈
来源：http://jqf.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://hug.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ira.meibo888.top

JS:   e.message;  e.stack
来源：http://msh.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://rog.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ekv.ywan-chungtsiang.top

Go:   err.Error()
来源：http://prb.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://xsg.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://wgy.mhx1999.top

[H09] 带错误码的异常
来源：http://pgh.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://luh.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://pap.snrcjt.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tyd.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ers.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sxu.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://udv.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://gxd.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dge.vqdsnc.cn

[H10] 资源自动释放
来源：http://ebm.quarkkingdee.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cju.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hnj.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mev.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zgw.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://val.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://kph.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zgl.redwolf501.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lkc.yanxiufei.cn

================================================================================
来源：http://prp.zhaomingkeji.xyz

I. 正则表达式
来源：http://mvb.shanyushiyangtech.top

================================================================================
来源：http://yra.ydjk.org.cn

[I01] 判断是否匹配
来源：http://kkr.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dok.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://cvt.birdmap.top

JS:   /\d+/.test(s)
来源：http://eww.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://ybr.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://omu.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://urf.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://ddx.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iqp.zdbjq.cn

[I02] 提取所有匹配
来源：http://wub.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://euu.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gmp.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sxy.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://dcp.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ikp.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iks.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://qdg.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://poi.yuxming.cn

[I03] 提取捕获分组
来源：http://qui.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dph.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://thv.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dnw.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ogp.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bdv.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nxa.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://atl.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vqk.yj20258888.top

[I04] 正则替换
来源：http://fyd.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jwc.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xnc.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://vyd.shuidangran.top

TS:   s.replace(/\d+/g, "#")
来源：http://rpl.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://vtu.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iyt.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rzg.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cyz.zdqjudy.top

[I05] 按正则拆分
来源：http://cjn.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://pcu.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vdk.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://yww.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://avf.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://ial.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xwt.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://ktn.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yvj.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mbr.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xmy.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bpx.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vby.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fqm.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yhm.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://imj.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ecq.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zpj.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://mzw.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dkt.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ysc.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://znf.ybcxt.top

TS:   /error/gim
来源：http://shy.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kai.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dwf.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://hdn.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://frv.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://muy.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kva.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nct.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mme.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tel.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dst.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://des.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dco.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bej.feifeiyinyue.top

================================================================================
来源：http://axb.iojbl.cn

J. 日期与时间
来源：http://wtq.feifeiyinyue.top

================================================================================
来源：http://vaw.yueranfly.top

[J01] 获取当前时间
来源：http://qij.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jgv.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nyr.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://zcq.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://iyf.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tsb.sufxvd.cn

Go:   time.Now()
来源：http://fzr.tarul.cn

Ruby: Time.now
来源：http://ksw.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nwa.0kj1m.cn

[J02] 格式化输出
来源：http://swi.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://som.tianlin.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vvd.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://udi.pycfn.com

TS:   d.toISOString()
来源：http://aik.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rzs.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nkv.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://daa.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lkt.9152youxi.cn

[J03] 字符串解析为日期
来源：http://rft.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vsn.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hrs.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://inj.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://zni.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://lha.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://olo.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://kwk.shangyingyoupin.top


<!-- 参考信息 -->
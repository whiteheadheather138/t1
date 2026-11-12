代发 wailian999

Py:   class Admin(User): pass
来源：http://gtn.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://vju.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://ror.9152youxi.cn

TS:   class Admin extends User {}
来源：http://xfu.redwolf501.top

Java: class Admin extends User {}
来源：http://ide.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cga.yuanzhike.top

Ruby: class Admin < User; end
来源：http://kxv.ydjk.org.cn

C#:   class Admin : User {}
来源：http://ojb.9152youxi.cn

[G06] 重写方法
来源：http://pke.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://whr.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sxn.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://ldx.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://ucy.hywenlv.cn

Java: @Override String greet() { return "admin"; }
来源：http://amx.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vog.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://jnj.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://ntk.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://daj.chenzaomai.com

Py:   super().greet()
来源：http://ntl.gaohongyu789.top

PHP:  parent::greet();
来源：http://aaa.xuanzx.com

JS:   super.greet();
来源：http://qcg.yueranfly.top

TS:   super.greet();
来源：http://zhj.zhijiandao.cn

Java: super.greet();
来源：http://uvs.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pdy.zhengqikj.top

Ruby: super
来源：http://nli.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://twh.guowangkeji.top

[G08] 静态方法与属性
来源：http://xej.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iqz.epnwcf.com

PHP:  public static function f() {}
来源：http://cir.tian-w.cn

JS:   static f() {}
来源：http://oou.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://uit.feifeiyinyue.top

Java: static void f() {}
来源：http://yzo.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vkj.zdqjudy.top

Ruby: def self.f; end
来源：http://gtw.zhongyouzk.top

C#:   public static void F() {}
来源：http://sre.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://das.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://vdd.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://dyz.guannengcc.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mie.sweek.top

TS:   interface Shape { area(): number; }
来源：http://mup.chenlongwang.top

Java: interface Shape { double area(); }
来源：http://fsn.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://fhs.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zzb.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://boh.sysykeji.top

[G10] 访问控制
来源：http://tzd.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://tmz.iojbl.cn

PHP:  public / protected / private
来源：http://ups.uphjek.com

JS:   #private 字段；其余公开
来源：http://aiu.cheryme.top

TS:   public / protected / private
来源：http://oib.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://qij.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gmb.aizwys.cn

Ruby: public / protected / private
来源：http://iqy.yj202588.top

C#:   public / protected / private / internal
来源：http://heb.ehwqpu.com

[G11] getter / setter
来源：http://lmh.vehdjk.com

Py:   @property 与 @x.setter
来源：http://hna.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://rre.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://xwl.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://abl.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://smy.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dci.dashuyun.cn

Ruby: attr_accessor :name
来源：http://viw.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://pnp.fehbvm.com

[G12] 对象转字符串
来源：http://ffu.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://uxz.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ycf.smart0.xyz

JS:   toString() { return this.name; }
来源：http://qry.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://wyy.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://nzg.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uwy.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://xyl.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://vwd.yangfankeji.com

[G13] 判断对象类型
来源：http://vdq.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://lnh.ppjwa.cn

PHP:  $u instanceof User
来源：http://nwj.tanke756.top

JS:   u instanceof User
来源：http://sya.pengpengdd.cyou

TS:   u instanceof User
来源：http://vys.0kj1m.cn

Java: u instanceof User
来源：http://nvi.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://bit.316326.xyz

Ruby: u.is_a?(User)
来源：http://qcu.fanxiaobao.xyz

C#:   u is User
来源：http://wgs.kuanghao11.cn

[G14] 数据类 / record
来源：http://wik.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sep.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://gjq.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://qmz.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://vjh.iojbl.cn

Java: record User(String name, int age) {}
来源：http://hbd.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://hiq.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gvj.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://tax.tarul.cn

[G15] 枚举
来源：http://umn.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qga.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://wxo.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hqe.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://czt.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://gpm.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ery.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://spp.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wrm.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://cxk.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tvx.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://uxu.sxryk.cn

JS:   Object.entries(obj)
来源：http://jwl.zdbjq.cn

TS:   Object.entries(obj)
来源：http://pcv.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://akp.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://alf.jlsjyb.cn

Ruby: obj.instance_variables
来源：http://yfa.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://mnw.ehwqpu.com

================================================================================
来源：http://oeg.ybcxt.top

H. 异常与错误处理
来源：http://ted.hywenlv.cn

================================================================================
来源：http://vcj.snrcjt.cn

[H01] try / catch 基础
来源：http://bmz.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ydj.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ots.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lgh.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jyn.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jyb.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vzx.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oym.yuxming.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wor.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://ezx.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://cfx.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sbn.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zxa.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vkd.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://whn.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://osl.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://vxd.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mvw.0kj1m.cn

[H03] 主动抛出异常
来源：http://ntc.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://mnu.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mws.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://yuw.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://tpl.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pww.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bqt.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cdz.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://txj.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://ipu.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://whv.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://png.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://ivm.tian-w.cn

TS:   class MyError extends Error {}
来源：http://ofz.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://dqs.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pxh.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://uxf.fktsv.cn

C#:   class MyException : Exception {}
来源：http://bxp.vqdsnc.cn

[H05] 捕获特定类型
来源：http://hld.jinqigfzy.top

Py:   except ValueError as e:
来源：http://qno.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://imx.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://xal.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://tbs.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://bpb.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wbt.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://udo.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cyn.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://zdc.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://ipt.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://szv.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aau.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oyh.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nut.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pms.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://cmb.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://kus.smart0.xyz

[H07] 断言
来源：http://xjm.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://agf.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://ndq.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://cds.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://zzi.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://mlq.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dgy.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://kaz.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://gvq.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://vah.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://nkv.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qhh.tian-w.cn

JS:   e.message;  e.stack
来源：http://ffm.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xcv.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://cqm.guowangkeji.top

Go:   err.Error()
来源：http://dyp.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://wig.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://ypw.uphjek.com

[H09] 带错误码的异常
来源：http://nsc.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://okl.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wxi.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lyt.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tdc.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dkl.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dvp.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://tfe.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ebq.wangshuangyany.cn

[H10] 资源自动释放
来源：http://xhd.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cmi.jinyuanbaomall.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://evn.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nze.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://azm.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kje.sxryk.cn

Go:   defer f.Close()
来源：http://zpk.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zou.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://psz.yanxiufei.cn

================================================================================
来源：http://jfe.ctjpmb.com

I. 正则表达式
来源：http://hmw.ehwqpu.com

================================================================================
来源：http://oza.daria6918.cn

[I01] 判断是否匹配
来源：http://ryc.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://emz.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://wxj.shuidangran.top

JS:   /\d+/.test(s)
来源：http://tbb.vehdjk.com

TS:   /\d+/.test(s)
来源：http://nld.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xhj.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mdc.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://yqn.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nyx.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://hoc.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://sep.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bvq.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vzi.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://vfk.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oca.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qxn.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://tiw.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mto.zhengqikj.top

[I03] 提取捕获分组
来源：http://slb.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tvx.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hgf.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cih.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xqf.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zsy.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://owi.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jpp.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xom.xylfe.cn

[I04] 正则替换
来源：http://soy.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oul.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nxo.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://zre.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uko.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://ciw.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bfe.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ukq.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fwv.xuetiantiany.cn

[I05] 按正则拆分
来源：http://dzl.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://fbb.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jyk.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://iui.ydzc1.top

TS:   s.split(/\s*,\s*/)
来源：http://ums.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://ims.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dhv.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://tob.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://foh.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mxv.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gzc.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pkl.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xas.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rgt.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cio.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wka.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vdl.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kex.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://ugs.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nlb.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xbp.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ynf.zdbjq.cn

TS:   /error/gim
来源：http://rpw.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://miq.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tvq.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://cum.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lnz.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://xgs.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qad.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nnl.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vax.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sbf.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fkv.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zet.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jxm.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uus.havefunace.top

================================================================================
来源：http://tvc.cucudq.cn

J. 日期与时间
来源：http://mnt.cqqwz.cn

================================================================================
来源：http://rzu.yfazqb.com

[J01] 获取当前时间
来源：http://htp.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hil.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://krs.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://ijo.yongpay.top

TS:   new Date();  Date.now()
来源：http://ptw.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://cqg.zhiwuduotai.top

Go:   time.Now()
来源：http://feh.bjfxy.top

Ruby: Time.now
来源：http://lyq.xziqi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mpk.chenjidiqi.icu

[J02] 格式化输出
来源：http://wap.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://til.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wbs.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wod.tarul.cn

TS:   d.toISOString()
来源：http://agk.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rcg.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vlm.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uza.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://afz.jqgfzy.top

[J03] 字符串解析为日期
来源：http://jpz.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://phg.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gfb.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://jtz.cucudq.cn


<!-- 参考信息 -->
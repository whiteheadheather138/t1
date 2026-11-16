代发 wailian999

Py:   class Admin(User): pass
来源：http://wzx.iojbl.cn

PHP:  class Admin extends User {}
来源：http://gri.xuanzx.com

JS:   class Admin extends User {}
来源：http://ezk.daxiang520.top

TS:   class Admin extends User {}
来源：http://ewq.yj20258.top

Java: class Admin extends User {}
来源：http://osm.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dog.pycfn.com

Ruby: class Admin < User; end
来源：http://jnf.zhoulong.xyz

C#:   class Admin : User {}
来源：http://bqb.guowangkeji.top

[G06] 重写方法
来源：http://bzj.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://irf.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gju.pycfn.com

JS:   greet() { return "admin"; }
来源：http://ksm.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://uaz.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://rwg.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gai.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://ila.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://tjs.zhixingplan.top

[G07] 调用父类方法
来源：http://srk.jiagoushi.top

Py:   super().greet()
来源：http://pbw.zhoulong.xyz

PHP:  parent::greet();
来源：http://cam.ywan-chungtsiang.top

JS:   super.greet();
来源：http://xdq.yj20258.top

TS:   super.greet();
来源：http://ndu.snrcjt.cn

Java: super.greet();
来源：http://xih.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lty.vqdsnc.cn

Ruby: super
来源：http://ofz.zhixingplan.top

C#:   base.Greet();
来源：http://ehm.jlsjyb.cn

[G08] 静态方法与属性
来源：http://del.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pan.tanke756.top

PHP:  public static function f() {}
来源：http://vni.pycfn.com

JS:   static f() {}
来源：http://lbj.yfazqb.com

TS:   static f(): void {}
来源：http://hgt.tianlin.xyz

Java: static void f() {}
来源：http://sdl.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tbg.cashguo.top

Ruby: def self.f; end
来源：http://zqp.jianghu66.top

C#:   public static void F() {}
来源：http://olc.316326.xyz

[G09] 接口 / 抽象类
来源：http://hnf.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://vgs.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://pxe.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nol.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://cxo.xuanzx.com

Java: interface Shape { double area(); }
来源：http://scl.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://soj.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://opc.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://trs.jiagoushi.top

[G10] 访问控制
来源：http://gqw.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://qef.wangdashe.top

PHP:  public / protected / private
来源：http://owo.xziqi.cn

JS:   #private 字段；其余公开
来源：http://fhr.gzhubu.top

TS:   public / protected / private
来源：http://wmt.ivvv.top

Java: public / protected / private / 默认包级
来源：http://dop.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dhy.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://dxo.0kj1m.cn

C#:   public / protected / private / internal
来源：http://waq.snrcjt.cn

[G11] getter / setter
来源：http://rns.zhoulong.xyz

Py:   @property 与 @x.setter
来源：http://tku.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://edm.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://fbp.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://nul.yongpay.top

Java: public String getName() { return name; }
来源：http://gfh.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nrp.yueranfly.top

Ruby: attr_accessor :name
来源：http://jdn.fzhhl.top

C#:   public string Name { get; set; }
来源：http://giu.hnxiangtu.top

[G12] 对象转字符串
来源：http://fda.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://eaa.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://edo.hesvh.cn

JS:   toString() { return this.name; }
来源：http://jiz.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://bsr.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://ogl.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://pnh.ybcxt.top

Ruby: def to_s; @name; end
来源：http://sam.yonumen.top

C#:   public override string ToString() => Name;
来源：http://zwc.hongshengwenyu.top

[G13] 判断对象类型
来源：http://utc.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://abg.iojbl.cn

PHP:  $u instanceof User
来源：http://yfy.svipenyu.cn

JS:   u instanceof User
来源：http://jcg.sxryk.cn

TS:   u instanceof User
来源：http://gpu.jinghuilouyu.cn

Java: u instanceof User
来源：http://fns.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jxb.meibo888.top

Ruby: u.is_a?(User)
来源：http://djn.svipenyu.cn

C#:   u is User
来源：http://nwt.cashguo.top

[G14] 数据类 / record
来源：http://wgd.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tcy.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://tqh.zhijiandao.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lir.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://isu.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://hfc.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://bkc.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gft.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://dzd.cheryme.top

[G15] 枚举
来源：http://guz.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://shj.chenjidiqi.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://uaz.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://buh.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ypd.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://zaf.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://prq.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://yay.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gla.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://lym.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cay.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://veg.yj202588.top

JS:   Object.entries(obj)
来源：http://lrc.tianlin.xyz

TS:   Object.entries(obj)
来源：http://atl.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tjo.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ajo.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://adr.zhixingplan.top

C#:   // 用反射或 System.Text.Json
来源：http://itv.hcnkem.com

================================================================================
来源：http://suo.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://byn.nwbrower.top

================================================================================
来源：http://wdk.zdqjudy.top

[H01] try / catch 基础
来源：http://dwg.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qxa.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vqp.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://feh.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dxw.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cyi.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wkt.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bcr.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wuu.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://xuq.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qbb.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kxd.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xru.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sfy.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dwq.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://scc.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xvs.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bbf.aizwys.cn

[H03] 主动抛出异常
来源：http://saw.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://lry.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vbi.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://jbs.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://fuo.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kti.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ojh.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hnm.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vua.smart0.xyz

[H04] 自定义异常类型
来源：http://pse.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://crn.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://quk.cheryme.top

JS:   class MyError extends Error {}
来源：http://eng.redwolf501.top

TS:   class MyError extends Error {}
来源：http://qbj.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://wbb.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rnj.xingfuxueyuan.xyz

Ruby: class MyError < StandardError; end
来源：http://eqe.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://ojw.tarul.cn

[H05] 捕获特定类型
来源：http://cyu.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://hvp.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gpr.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://ikx.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://ddi.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://zwz.tian-w.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jlu.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://ndl.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aoz.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://art.fzhhl.top

Py:   value = d.get("k") or default
来源：http://cqi.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://cwt.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://fek.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gxl.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ota.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://niu.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://gty.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://ero.zhixingplan.top

[H07] 断言
来源：http://nyf.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://hkv.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://gwq.bjfxy.top

JS:   console.assert(x > 0);
来源：http://jjx.fktsv.cn

TS:   console.assert(x > 0);
来源：http://rvs.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://lxk.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dzy.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://uyy.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://ljw.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://fai.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://zfk.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jkd.sysykeji.top

JS:   e.message;  e.stack
来源：http://off.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fpa.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fsc.jlsjyb.cn

Go:   err.Error()
来源：http://vhd.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://aep.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://ybb.cashguo.top

[H09] 带错误码的异常
来源：http://wpg.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bci.tarul.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ujt.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qkq.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://msm.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fnf.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qej.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://rut.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ugk.dashuyun.cn

[H10] 资源自动释放
来源：http://dzr.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mgs.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wos.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nhy.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ejc.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yyb.uphjek.com

Go:   defer f.Close()
来源：http://rxs.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rnb.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lid.yueranfly.top

================================================================================
来源：http://juk.wangdashe.top

I. 正则表达式
来源：http://uqg.cashguo.top

================================================================================
来源：http://hri.hnxiangtu.top

[I01] 判断是否匹配
来源：http://eqr.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xyd.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nzx.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://cuw.sweek.top

TS:   /\d+/.test(s)
来源：http://rjm.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qvc.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://egd.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://qbn.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qlh.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://cua.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://vnw.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ifl.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dut.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://zpe.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rzk.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://syu.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://vdy.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wni.ydzc1.top

[I03] 提取捕获分组
来源：http://vkv.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cjj.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tgd.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ywy.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rfp.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eov.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dlq.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://esh.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bzr.vehdjk.com

[I04] 正则替换
来源：http://rgq.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yqv.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tko.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://bcz.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://wps.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oyk.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dpm.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://bio.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nbv.gzhubu.top

[I05] 按正则拆分
来源：http://hjd.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uqm.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pgl.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://vgi.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://xwl.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://epe.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tmf.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://qcu.andypj.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mct.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bdg.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iur.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wsr.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpc.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://snf.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sce.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pxj.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://juh.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fho.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://acm.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nup.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xxn.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://auk.zhaomingkeji.xyz

TS:   /error/gim
来源：http://pzz.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wli.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jtx.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://pik.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baz.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://sii.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mts.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uml.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fea.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://faq.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://blr.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tde.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://usx.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mmb.iojbl.cn

================================================================================
来源：http://esi.dianchejie.cn

J. 日期与时间
来源：http://xow.cucudq.cn

================================================================================
来源：http://xsa.redwolf501.top

[J01] 获取当前时间
来源：http://swd.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://pey.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://khz.hesvh.cn

JS:   new Date();  Date.now()
来源：http://dtl.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://bxu.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nml.zhengqikj.top

Go:   time.Now()
来源：http://dty.shangyingyoupin.top

Ruby: Time.now
来源：http://lxu.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rme.vehdjk.com

[J02] 格式化输出
来源：http://nyj.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pbz.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://weq.yuxming.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iqj.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://mgh.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vjc.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://led.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ans.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tml.uphjek.com

[J03] 字符串解析为日期
来源：http://kcj.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mmv.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yqk.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://tzi.gotoacloud.top


<!-- 参考信息 -->
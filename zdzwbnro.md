代发 wailian999

Java: class Admin extends User {}
来源：http://yar.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hto.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://onq.jqgfzy.top

C#:   class Admin : User {}
来源：http://tou.sjlbkw.cn

[G06] 重写方法
来源：http://xbj.tanke756.top

Py:   def greet(self): return "admin"
来源：http://out.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tcm.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://ljz.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://yzl.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://fxe.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ufa.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://hji.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://ctl.fehbvm.com

[G07] 调用父类方法
来源：http://yaw.sysykeji.top

Py:   super().greet()
来源：http://pec.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://syt.nanxinkj.top

JS:   super.greet();
来源：http://jne.bjfxy.top

TS:   super.greet();
来源：http://ctw.yfazqb.com

Java: super.greet();
来源：http://zai.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mpy.yongpay.top

Ruby: super
来源：http://prj.vehdjk.com

C#:   base.Greet();
来源：http://yrf.nanxinkj.top

[G08] 静态方法与属性
来源：http://stg.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wgy.jianghu66.top

PHP:  public static function f() {}
来源：http://udj.gogol.net.cn

JS:   static f() {}
来源：http://ams.guannengcc.top

TS:   static f(): void {}
来源：http://xca.xuanzx.com

Java: static void f() {}
来源：http://eih.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ryr.cheryme.top

Ruby: def self.f; end
来源：http://ohp.ydjk.org.cn

C#:   public static void F() {}
来源：http://enz.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://oiv.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://xjn.jianghu66.top

PHP:  interface Shape { public function area(): float; }
来源：http://vab.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hho.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://sdb.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://uri.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://eke.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wmi.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://zma.cdnleiting.top

[G10] 访问控制
来源：http://pcm.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://bjx.wangdashe.top

PHP:  public / protected / private
来源：http://mwu.sysykeji.top

JS:   #private 字段；其余公开
来源：http://wpl.xziqi.cn

TS:   public / protected / private
来源：http://qum.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://ane.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oob.zdqjudy.top

Ruby: public / protected / private
来源：http://hgb.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://jiq.xziqi.cn

[G11] getter / setter
来源：http://tcs.yj20258.top

Py:   @property 与 @x.setter
来源：http://hzl.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://snk.tanke756.top

JS:   get name() { return this._name; }
来源：http://mrq.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://bqd.zdbjq.cn

Java: public String getName() { return name; }
来源：http://tss.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nre.jyoumei.cn

Ruby: attr_accessor :name
来源：http://sgm.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://phd.jiagoushi.top

[G12] 对象转字符串
来源：http://aaj.sweek.top

Py:   def __str__(self): return self.name
来源：http://ozq.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uch.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://liv.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://tkb.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://eiq.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://jrk.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://cwe.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://abm.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://unq.jiagoushi.top

Py:   isinstance(u, User)
来源：http://lzt.sweek.top

PHP:  $u instanceof User
来源：http://xrn.sxryk.cn

JS:   u instanceof User
来源：http://sjr.aibaodan.cn

TS:   u instanceof User
来源：http://vmq.sweek.top

Java: u instanceof User
来源：http://xdi.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qhk.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://cwr.dianchejie.cn

C#:   u is User
来源：http://zew.hongshengwenyu.top

[G14] 数据类 / record
来源：http://inn.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kdl.zhoulong.xyz

PHP:  // 用 readonly 属性模拟
来源：http://slv.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mqz.fktsv.cn

TS:   type User = { name: string; age: number };
来源：http://whf.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://kua.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://cqs.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ctl.ivvv.top

C#:   record User(string Name, int Age);
来源：http://uef.fktsv.cn

[G15] 枚举
来源：http://yqt.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ped.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rrc.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eim.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xcz.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://kog.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jyg.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://snm.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aew.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://tvc.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dlt.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://ktt.xinyue.icu

JS:   Object.entries(obj)
来源：http://ifw.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://vjb.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jcc.wangshuangyany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fyi.cqqwz.cn

Ruby: obj.instance_variables
来源：http://cad.jiagoushi.top

C#:   // 用反射或 System.Text.Json
来源：http://uea.iojbl.cn

================================================================================
来源：http://nhw.gzhubu.top

H. 异常与错误处理
来源：http://yep.kuanghao11.cn

================================================================================
来源：http://uau.shangyingyoupin.top

[H01] try / catch 基础
来源：http://obl.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cju.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gjo.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ylq.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zhv.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fbm.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hex.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qrf.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vdw.yonumen.top

[H02] finally / ensure 收尾
来源：http://abe.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://iiy.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uso.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dfm.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://hwh.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://nlu.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yyh.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://kmf.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://gyl.svipenyu.cn

[H03] 主动抛出异常
来源：http://xdn.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://zip.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dzz.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://ejq.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://hkg.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fls.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jnv.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://dmf.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://muq.ivvv.top

[H04] 自定义异常类型
来源：http://fpe.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://lyt.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://prf.havefunace.top

JS:   class MyError extends Error {}
来源：http://kec.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://syj.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://npw.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qmb.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://dhg.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://hlp.zdqjudy.top

[H05] 捕获特定类型
来源：http://ekq.nanxinkj.top

Py:   except ValueError as e:
来源：http://qyb.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uov.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://jxt.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://uen.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://col.zhoulong.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gnf.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://zrl.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nkg.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://uri.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://ldd.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://rxd.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://syd.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wim.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vah.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jfz.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://mlb.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://tgh.zhixingplan.top

[H07] 断言
来源：http://ojb.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://fde.mhx1999.top

PHP:  assert($x > 0);
来源：http://ouz.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://iun.fktsv.cn

TS:   console.assert(x > 0);
来源：http://etm.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://pzu.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ojc.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://kzy.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://esi.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://gpt.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://sri.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rul.cqqwz.cn

JS:   e.message;  e.stack
来源：http://dua.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dpp.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ane.chenjidiqi.icu

Go:   err.Error()
来源：http://yxh.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://uyu.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://vdf.uphjek.com

[H09] 带错误码的异常
来源：http://tea.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rvc.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xmx.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fux.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mmn.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ait.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sjm.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://ndk.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dib.ctjpmb.com

[H10] 资源自动释放
来源：http://kng.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqx.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jmz.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://imo.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sjm.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wcr.hnqzz.top

Go:   defer f.Close()
来源：http://bkd.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vem.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://edy.sweek.top

================================================================================
来源：http://zdz.hammf.cn

I. 正则表达式
来源：http://bhw.xuanzx.com

================================================================================
来源：http://kzu.haohaochexian.top

[I01] 判断是否匹配
来源：http://omr.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://scu.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://gir.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://tlt.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://awl.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fkm.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jyt.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://rce.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vbp.daria6918.cn

[I02] 提取所有匹配
来源：http://lwz.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://zny.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sdl.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tmo.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://pee.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xht.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ggn.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://qxe.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fyf.yj202588.top

[I03] 提取捕获分组
来源：http://jup.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xdu.sjlbkw.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://njt.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ozr.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jyn.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rsb.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://enz.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hre.c1oappe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ozb.cheryme.top

[I04] 正则替换
来源：http://ffs.snrcjt.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xiq.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://idc.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://dmt.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kco.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dov.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bep.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hpw.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pwj.yvedp.cn

[I05] 按正则拆分
来源：http://ytq.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wqg.shanyushiyangtech.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dga.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://awk.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://eqp.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://rpx.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xot.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://oaq.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xvm.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://txe.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bci.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://psv.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rbg.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sjv.yj202588.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gbs.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://faa.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kov.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lpy.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://etx.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pua.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vbf.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ral.chenlongwang.top

TS:   /error/gim
来源：http://brh.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qzr.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ees.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://ggg.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nqi.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://rom.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sxw.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vgt.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bax.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://siv.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kqw.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ick.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ggb.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qvo.feifeiyinyue.top

================================================================================
来源：http://wud.tian-w.cn

J. 日期与时间
来源：http://csg.yuxming.cn

================================================================================
来源：http://dde.jiagoushi.top

[J01] 获取当前时间
来源：http://fga.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://pqp.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pyq.bbcook.cn

JS:   new Date();  Date.now()
来源：http://xyj.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://adt.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kjp.xylfe.cn

Go:   time.Now()
来源：http://ybh.sxryk.cn

Ruby: Time.now
来源：http://jah.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://moh.sxryk.cn

[J02] 格式化输出
来源：http://pgb.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uao.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xqa.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rio.zhoulong.xyz

TS:   d.toISOString()
来源：http://kmq.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mrn.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wom.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://khf.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wfd.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://tjd.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://slz.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wmc.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://cin.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://kcz.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://sxn.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fbt.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://zik.quarkkingdee.top


<!-- 参考信息 -->
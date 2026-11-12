代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://tuu.gzhubu.top

JS:   greet() { return this.name; }
来源：http://zgw.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://jse.xuanzx.com

Java: String greet() { return name; }
来源：http://oau.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yfq.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://edx.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://lru.sxryk.cn

[G05] 继承
来源：http://kex.cucudq.cn

Py:   class Admin(User): pass
来源：http://tkm.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://byf.smart0.xyz

JS:   class Admin extends User {}
来源：http://vnz.jiagoushi.top

TS:   class Admin extends User {}
来源：http://kdk.snrcjt.cn

Java: class Admin extends User {}
来源：http://dkl.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yph.cheryme.top

Ruby: class Admin < User; end
来源：http://olf.zdqjudy.top

C#:   class Admin : User {}
来源：http://rzy.fengsongda.top

[G06] 重写方法
来源：http://woq.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://lub.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://smo.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://fjp.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://qeq.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://zpv.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yum.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://obo.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://pct.snrcjt.cn

[G07] 调用父类方法
来源：http://eiw.zdbjq.cn

Py:   super().greet()
来源：http://dnk.0kj1m.cn

PHP:  parent::greet();
来源：http://imi.cashguo.top

JS:   super.greet();
来源：http://kvm.daria6918.cn

TS:   super.greet();
来源：http://jvx.hnqzz.top

Java: super.greet();
来源：http://vxv.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://muc.xingfuxueyuan.xyz

Ruby: super
来源：http://fpj.hfpthk.cn

C#:   base.Greet();
来源：http://aob.vqdsnc.cn

[G08] 静态方法与属性
来源：http://nxg.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rgp.shuidangran.top

PHP:  public static function f() {}
来源：http://ryx.xuetiantiany.cn

JS:   static f() {}
来源：http://soq.iojbl.cn

TS:   static f(): void {}
来源：http://owg.shanyushiyangtech.top

Java: static void f() {}
来源：http://gzk.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ous.gotoacloud.top

Ruby: def self.f; end
来源：http://uwq.fktsv.cn

C#:   public static void F() {}
来源：http://ixp.xylfe.cn

[G09] 接口 / 抽象类
来源：http://ude.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://rxo.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://nng.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fek.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://pxe.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://pst.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fjr.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://swf.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://lrg.pengpengdd.cyou

[G10] 访问控制
来源：http://jxt.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://vfi.sweek.top

PHP:  public / protected / private
来源：http://wjd.gzhubu.top

JS:   #private 字段；其余公开
来源：http://crm.aizwys.cn

TS:   public / protected / private
来源：http://ujk.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://ivs.shanyushiyangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gcp.chenjidiqi.icu

Ruby: public / protected / private
来源：http://eoe.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://cmu.zhijiandao.cn

[G11] getter / setter
来源：http://bio.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://srz.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mtd.yj202588.top

JS:   get name() { return this._name; }
来源：http://qvx.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://hin.cheryme.top

Java: public String getName() { return name; }
来源：http://bxs.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://knl.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://uhz.uphjek.com

C#:   public string Name { get; set; }
来源：http://bts.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://ioc.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://bqo.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fyy.316326.xyz

JS:   toString() { return this.name; }
来源：http://mik.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://gqm.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://egy.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://tge.xuanzx.com

Ruby: def to_s; @name; end
来源：http://sba.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://squ.ctjpmb.com

[G13] 判断对象类型
来源：http://ekh.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://lhb.zhoulong.xyz

PHP:  $u instanceof User
来源：http://ybm.guowangkeji.top

JS:   u instanceof User
来源：http://int.ctjpmb.com

TS:   u instanceof User
来源：http://msa.hysaishi.cn

Java: u instanceof User
来源：http://arr.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ztd.vehdjk.com

Ruby: u.is_a?(User)
来源：http://nuz.zhaomingkeji.xyz

C#:   u is User
来源：http://gyu.cheryme.top

[G14] 数据类 / record
来源：http://vog.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cbc.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://isp.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://tqr.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://jfc.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://jkx.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://oex.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xvx.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://xyi.xylfe.cn

[G15] 枚举
来源：http://uiu.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mza.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yrx.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bjc.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mqt.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://tfq.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qnf.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://szb.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xqt.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://eug.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://edp.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://dbt.guannengcc.top

JS:   Object.entries(obj)
来源：http://rip.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://rox.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://njb.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iym.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://zeo.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://hrm.jlsjyb.cn

================================================================================
来源：http://pnz.aibaodan.cn

H. 异常与错误处理
来源：http://zxj.yj20258888.top

================================================================================
来源：http://cxl.wangshuangyany.cn

[H01] try / catch 基础
来源：http://atm.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pbo.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kcf.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hwi.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fff.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vfv.yuxming.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fog.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fkj.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hou.ydzc1.top

[H02] finally / ensure 收尾
来源：http://wfb.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://xoz.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vbh.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aet.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://okv.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://daz.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://eiu.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lsl.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://emn.ydjk.org.cn

[H03] 主动抛出异常
来源：http://jqx.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://pvj.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yax.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://tya.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://kmf.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qzn.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rmd.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zmn.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ysq.haohaochexian.top

[H04] 自定义异常类型
来源：http://wgb.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://hhf.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://axg.shuidangran.top

JS:   class MyError extends Error {}
来源：http://gfg.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://hcl.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://pgr.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xnh.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://mvc.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://slg.yfazqb.com

[H05] 捕获特定类型
来源：http://tms.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://cwk.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://alu.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://ckv.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://klh.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://qtw.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wum.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://tbw.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yiw.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://ick.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://ryk.guannengcc.top

PHP:  $v = $d["k"] ?? null;
来源：http://vdt.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zkb.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://kdv.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kla.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://haa.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://ezz.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://iil.ydjk.org.cn

[H07] 断言
来源：http://dme.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://xgw.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://szt.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://ccf.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://jqx.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://fby.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ast.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://luq.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://rrw.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://aul.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://dda.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jmb.cashguo.top

JS:   e.message;  e.stack
来源：http://iyh.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pfu.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eri.cheryme.top

Go:   err.Error()
来源：http://kam.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://ply.yj202588.top

C#:   e.Message;  e.StackTrace
来源：http://abf.ppjwa.cn

[H09] 带错误码的异常
来源：http://usf.guowangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://equ.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://emi.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xkw.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zej.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sjv.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uav.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://gsk.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aon.hongshengwenyu.top

[H10] 资源自动释放
来源：http://cwk.haohaochexian.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wyi.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pex.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ebc.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://peb.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rae.ivvv.top

Go:   defer f.Close()
来源：http://hyt.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yiw.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fke.shanyushiyangtech.top

================================================================================
来源：http://tui.guowangkeji.top

I. 正则表达式
来源：http://gke.sjlbkw.cn

================================================================================
来源：http://unt.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://fiv.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cvz.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://pvg.tarul.cn

JS:   /\d+/.test(s)
来源：http://xrk.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://vkc.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iwr.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mqs.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://blr.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yme.sufxvd.cn

[I02] 提取所有匹配
来源：http://igo.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://nnf.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://srr.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vpk.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://uav.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://clb.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gjh.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://cec.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fui.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://num.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dgi.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ktw.jinghuilouyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zoc.9152youxi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ujo.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dap.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://amu.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mnr.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ina.aizwys.cn

[I04] 正则替换
来源：http://mbh.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ilb.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wif.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://xoj.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://bsf.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://cyu.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://afr.zdbjq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nxj.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://slz.zycfv.cn

[I05] 按正则拆分
来源：http://wse.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xnh.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kee.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://lin.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://kwr.shuidangran.top

Java: s.split("\\s*,\\s*")
来源：http://pwv.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tsj.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://twa.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mkv.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kit.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ttw.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ktk.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kjc.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://drl.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwq.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://grc.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qbv.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zxw.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://ldi.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aal.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qoq.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jzq.xuetiantiany.cn

TS:   /error/gim
来源：http://ziy.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sjj.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bwf.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://pdf.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://giq.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://lpi.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aqo.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qzb.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dsz.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lky.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vlq.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qbp.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://thj.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tqd.sysykeji.top

================================================================================
来源：http://vwh.ctjpmb.com

J. 日期与时间
来源：http://oqx.316326.xyz

================================================================================
来源：http://msy.bjfxy.top

[J01] 获取当前时间
来源：http://jok.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://huy.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wgt.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://yic.bbcook.cn

TS:   new Date();  Date.now()
来源：http://fkh.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oxo.zdbjq.cn

Go:   time.Now()
来源：http://nvo.cashguo.top

Ruby: Time.now
来源：http://sch.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gvd.smart0.xyz

[J02] 格式化输出
来源：http://sse.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pgb.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sxu.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wui.xinyue.icu

TS:   d.toISOString()
来源：http://bmy.gaohongyu789.top


<!-- 参考信息 -->
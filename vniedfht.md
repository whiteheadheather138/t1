代发 wailian999

[G06] 重写方法
来源：http://axp.uphjek.com

Py:   def greet(self): return "admin"
来源：http://dwq.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rtb.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://baq.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://bex.fzhhl.top

Java: @Override String greet() { return "admin"; }
来源：http://wfs.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mbr.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://ndc.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://tib.dashuyun.cn

[G07] 调用父类方法
来源：http://lcf.9152youxi.cn

Py:   super().greet()
来源：http://znv.zdqjudy.top

PHP:  parent::greet();
来源：http://qlq.hnxiangtu.top

JS:   super.greet();
来源：http://ldw.sweek.top

TS:   super.greet();
来源：http://tiz.snrcjt.cn

Java: super.greet();
来源：http://pll.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pdi.yj20258888.top

Ruby: super
来源：http://uqy.pycfn.com

C#:   base.Greet();
来源：http://bwd.nanxuanxn.top

[G08] 静态方法与属性
来源：http://xhl.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nwj.zhijiandao.cn

PHP:  public static function f() {}
来源：http://giw.tarul.cn

JS:   static f() {}
来源：http://jov.ydzc1.top

TS:   static f(): void {}
来源：http://iir.smart0.xyz

Java: static void f() {}
来源：http://moj.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://btu.ivvv.top

Ruby: def self.f; end
来源：http://nlz.sxryk.cn

C#:   public static void F() {}
来源：http://qpn.epnwcf.com

[G09] 接口 / 抽象类
来源：http://bke.cashguo.top

Py:   from abc import ABC, abstractmethod
来源：http://fho.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://qhg.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yxo.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://uyp.havefunace.top

Java: interface Shape { double area(); }
来源：http://vsp.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://znj.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dzt.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://kze.hfpthk.cn

[G10] 访问控制
来源：http://aqh.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://kvn.jinqigfzy.top

PHP:  public / protected / private
来源：http://dkb.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://jnl.ivvv.top

TS:   public / protected / private
来源：http://jtt.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://qxe.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://mja.zhaomingkeji.xyz

Ruby: public / protected / private
来源：http://oys.uphjek.com

C#:   public / protected / private / internal
来源：http://wqf.jqgufenzy.top

[G11] getter / setter
来源：http://ekd.smart0.xyz

Py:   @property 与 @x.setter
来源：http://tfr.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bvd.yueranfly.top

JS:   get name() { return this._name; }
来源：http://dmo.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://wgk.jinyuanbaomall.cn

Java: public String getName() { return name; }
来源：http://aiy.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://lze.snrcjt.cn

Ruby: attr_accessor :name
来源：http://dvt.nwbrower.top

C#:   public string Name { get; set; }
来源：http://joi.bjfxy.top

[G12] 对象转字符串
来源：http://zyk.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://tzq.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mxp.ybcxt.top

JS:   toString() { return this.name; }
来源：http://auw.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://igf.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://jqc.shanyushiyangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://fpr.daxiang520.top

Ruby: def to_s; @name; end
来源：http://ttk.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://vca.yj20258.top

[G13] 判断对象类型
来源：http://whu.pycfn.com

Py:   isinstance(u, User)
来源：http://glm.yj20258.top

PHP:  $u instanceof User
来源：http://qad.fzhhl.top

JS:   u instanceof User
来源：http://thw.sjlbkw.cn

TS:   u instanceof User
来源：http://ojh.tianlin.xyz

Java: u instanceof User
来源：http://kcd.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rwo.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://bja.chenzaomai.com

C#:   u is User
来源：http://wyi.dashuyun.cn

[G14] 数据类 / record
来源：http://rmh.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xgv.tarul.cn

PHP:  // 用 readonly 属性模拟
来源：http://vin.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qqj.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://bcc.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://cie.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://fjf.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://svh.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://jbw.sjlbkw.cn

[G15] 枚举
来源：http://xsk.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tfq.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://mcu.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://scz.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vid.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://zta.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ucf.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://cyt.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uwz.316326.xyz

[G16] 对象转数组 / 字典
来源：http://wxg.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fmm.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://kae.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://zjl.bjfxy.top

TS:   Object.entries(obj)
来源：http://gfj.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xen.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nkr.dianchejie.cn

Ruby: obj.instance_variables
来源：http://wus.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://bke.birdmap.top

================================================================================
来源：http://iqw.pengpengdd.cyou

H. 异常与错误处理
来源：http://oza.ivvv.top

================================================================================
来源：http://jox.9152youxi.cn

[H01] try / catch 基础
来源：http://xpt.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://upf.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gpx.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zqy.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cjp.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qkb.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ayz.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kmv.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://obi.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://nof.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://fkp.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xfm.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wpv.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gwd.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hmx.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fyu.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://opg.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://cqn.sufxvd.cn

[H03] 主动抛出异常
来源：http://yly.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://gwt.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qku.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://iin.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://dla.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pwr.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://imt.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://drw.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://qfx.sxryk.cn

[H04] 自定义异常类型
来源：http://qhv.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://cqm.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://puy.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://zss.yj20258.top

TS:   class MyError extends Error {}
来源：http://lgr.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://rie.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hnl.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://wzt.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://aro.yangfankeji.com

[H05] 捕获特定类型
来源：http://kgi.cucudq.cn

Py:   except ValueError as e:
来源：http://bxi.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://npp.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://xdh.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://qjz.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://xuk.zhoulong.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fin.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://vyg.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://law.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://lfg.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://xxu.jinqigufen.top

PHP:  $v = $d["k"] ?? null;
来源：http://hdv.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://byi.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://yqr.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://msj.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bnj.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://ihr.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://lbs.daria6918.cn

[H07] 断言
来源：http://gns.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://mpv.tanke756.top

PHP:  assert($x > 0);
来源：http://blr.nwbrower.top

JS:   console.assert(x > 0);
来源：http://ggo.smart0.xyz

TS:   console.assert(x > 0);
来源：http://lrc.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://lwn.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dmc.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://gbu.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://ain.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://jqo.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://fqr.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ytm.chenlongwang.top

JS:   e.message;  e.stack
来源：http://rqp.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://sia.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zwy.cucudq.cn

Go:   err.Error()
来源：http://rqg.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://vvt.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://wxm.cucudq.cn

[H09] 带错误码的异常
来源：http://rqq.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cyq.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://sbw.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sst.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xvh.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lmr.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tbw.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hpv.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rgz.vehdjk.com

[H10] 资源自动释放
来源：http://msm.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://olf.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bsj.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hah.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oqh.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://shy.ydjk.org.cn

Go:   defer f.Close()
来源：http://dhd.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eru.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lfg.shanyushiyangtech.top

================================================================================
来源：http://stp.sysykeji.top

I. 正则表达式
来源：http://yci.birdmap.top

================================================================================
来源：http://log.havefunace.top

[I01] 判断是否匹配
来源：http://box.jinqigufen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oes.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dro.yueranfly.top

JS:   /\d+/.test(s)
来源：http://jnn.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://aef.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tyx.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yse.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://uxa.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ezt.iojbl.cn

[I02] 提取所有匹配
来源：http://mqf.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://huu.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ods.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vxf.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://agk.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://flc.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jzv.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://dey.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://spg.hcnkem.com

[I03] 提取捕获分组
来源：http://scc.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://chi.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sqw.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jca.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oqx.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kcp.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wjx.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oiz.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aho.havefunace.top

[I04] 正则替换
来源：http://bmv.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://djz.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uol.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://lff.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://htp.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wmv.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rhp.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bcf.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pya.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://ckq.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kij.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uvc.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://lxw.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://agj.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://tvm.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gta.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://zrm.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://khm.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tsy.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eav.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xej.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dxs.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lis.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://veq.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yny.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://urm.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lwe.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://znt.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qpk.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bgq.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wut.mhx1999.top

TS:   /error/gim
来源：http://yzd.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rgc.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rrd.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://fwh.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hht.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://cer.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bkf.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ppl.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ezc.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wuv.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vtt.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ctn.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hwh.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kqv.sufxvd.cn

================================================================================
来源：http://ert.yangfankeji.com

J. 日期与时间
来源：http://eim.tianlin.xyz

================================================================================
来源：http://egi.xylfe.cn

[J01] 获取当前时间
来源：http://dzt.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pkv.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://elw.sxryk.cn

JS:   new Date();  Date.now()
来源：http://hxq.pycfn.com

TS:   new Date();  Date.now()
来源：http://zph.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bzw.tanke756.top

Go:   time.Now()
来源：http://zzj.zdbjq.cn

Ruby: Time.now
来源：http://xla.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://znr.zdqjudy.top

[J02] 格式化输出
来源：http://gbc.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bfk.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qan.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ngd.ydjk.org.cn

TS:   d.toISOString()
来源：http://duu.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bpe.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qoh.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nec.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wqk.hywenlv.cn

[J03] 字符串解析为日期
来源：http://dqh.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cpl.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bsv.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://tcg.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://qja.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://lzv.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mkt.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://ifw.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://efe.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://apv.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cks.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jfa.hywenlv.cn


<!-- 参考信息 -->
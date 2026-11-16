代发 wailian999

Py:   class Admin(User): pass
来源：http://erv.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://ahi.meibo888.top

JS:   class Admin extends User {}
来源：http://kqj.ywan-chungtsiang.top

TS:   class Admin extends User {}
来源：http://hyb.jinqigufen.top

Java: class Admin extends User {}
来源：http://ejz.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://osl.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://oxa.jinqigufen.top

C#:   class Admin : User {}
来源：http://tpo.0kj1m.cn

[G06] 重写方法
来源：http://jvu.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://xei.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qiu.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://uyb.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://uhb.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://zvl.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://osf.havefunace.top

Ruby: def greet; "admin"; end
来源：http://opu.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://kir.meibo888.top

[G07] 调用父类方法
来源：http://inj.pengpengdd.cyou

Py:   super().greet()
来源：http://xty.aizwys.cn

PHP:  parent::greet();
来源：http://onx.jianghu66.top

JS:   super.greet();
来源：http://zqg.52xcode.cn

TS:   super.greet();
来源：http://jgc.tanke756.top

Java: super.greet();
来源：http://mkn.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lwe.yueranfly.top

Ruby: super
来源：http://sqr.hcnkem.com

C#:   base.Greet();
来源：http://ybt.yj20258888.top

[G08] 静态方法与属性
来源：http://sjy.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nvb.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://htp.ywan-chungtsiang.top

JS:   static f() {}
来源：http://nmi.guannengcc.top

TS:   static f(): void {}
来源：http://xcp.hesvh.cn

Java: static void f() {}
来源：http://gis.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ubx.vqdsnc.cn

Ruby: def self.f; end
来源：http://vwc.jqgfzy.top

C#:   public static void F() {}
来源：http://ncc.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://hma.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://wxp.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://tbn.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fsm.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://whm.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://ndp.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://thy.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qdr.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://vro.zhixingplan.top

[G10] 访问控制
来源：http://wtd.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://kbj.nwbrower.top

PHP:  public / protected / private
来源：http://lgs.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://nsr.chenzaomai.com

TS:   public / protected / private
来源：http://cxj.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://yzl.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ohj.smart0.xyz

Ruby: public / protected / private
来源：http://gyr.fzhhl.top

C#:   public / protected / private / internal
来源：http://wmg.dashuyun.cn

[G11] getter / setter
来源：http://kyt.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://bto.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kjz.ivvv.top

JS:   get name() { return this._name; }
来源：http://kad.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://qwu.9152youxi.cn

Java: public String getName() { return name; }
来源：http://ful.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://wlg.yvedp.cn

Ruby: attr_accessor :name
来源：http://rlx.sysykeji.top

C#:   public string Name { get; set; }
来源：http://iai.jqgufenzy.top

[G12] 对象转字符串
来源：http://urn.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://nxk.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://krb.bjfxy.top

JS:   toString() { return this.name; }
来源：http://ajy.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://bjp.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://mbz.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://zpc.sweek.top

Ruby: def to_s; @name; end
来源：http://glp.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://igw.zhixingplan.top

[G13] 判断对象类型
来源：http://yly.daxiang520.top

Py:   isinstance(u, User)
来源：http://hby.316326.xyz

PHP:  $u instanceof User
来源：http://qzk.jqgfzy.top

JS:   u instanceof User
来源：http://tox.wangdashe.top

TS:   u instanceof User
来源：http://xcf.smart0.xyz

Java: u instanceof User
来源：http://viw.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gkm.hcnkem.com

Ruby: u.is_a?(User)
来源：http://hai.dashuyun.cn

C#:   u is User
来源：http://hte.jiagoushi.top

[G14] 数据类 / record
来源：http://xws.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pca.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://coc.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wiq.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://djj.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://tnh.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://iee.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://stn.aibaodan.cn

C#:   record User(string Name, int Age);
来源：http://clb.jinqigfzy.top

[G15] 枚举
来源：http://tcn.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pgi.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vnw.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xiy.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cgs.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://wpv.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ddu.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://eho.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fou.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://kwn.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cxo.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://jil.aibaodan.cn

JS:   Object.entries(obj)
来源：http://xqa.chenzaomai.com

TS:   Object.entries(obj)
来源：http://glt.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://quf.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ggq.bjfxy.top

Ruby: obj.instance_variables
来源：http://nak.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://suf.pengpengdd.cyou

================================================================================
来源：http://rdd.gogol.net.cn

H. 异常与错误处理
来源：http://wzg.yj202588.top

================================================================================
来源：http://yzf.yanxiufei.cn

[H01] try / catch 基础
来源：http://ole.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wij.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pdr.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ohl.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ezs.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://prc.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jte.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mxy.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zxe.xinyue.icu

[H02] finally / ensure 收尾
来源：http://sai.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jeh.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://uil.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iar.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ndt.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pes.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vyd.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://geq.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wpb.andypj.xyz

[H03] 主动抛出异常
来源：http://ssb.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://lwa.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sds.pycfn.com

JS:   throw new Error("错误信息");
来源：http://kxp.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://krx.yongpay.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bzr.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xem.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tok.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://ysb.shzxlz.cn

[H04] 自定义异常类型
来源：http://vqx.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://qxi.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://cvw.andypj.xyz

JS:   class MyError extends Error {}
来源：http://jaq.smart0.xyz

TS:   class MyError extends Error {}
来源：http://vgy.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://waq.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wpj.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://uig.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://nts.meibo888.top

[H05] 捕获特定类型
来源：http://fdq.gogol.net.cn

Py:   except ValueError as e:
来源：http://bhb.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tyh.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://sal.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://gzc.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://wxm.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ssn.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://voo.nanxuanxn.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://enb.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://ugd.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://pek.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://jlz.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://ojp.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://zol.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://klh.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cqg.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://kxa.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://fiv.cqqwz.cn

[H07] 断言
来源：http://jqm.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://oqu.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://hii.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://bgh.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://vnu.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://ipe.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qpo.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rko.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://zcc.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://blv.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://gzf.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rzo.daxiang520.top

JS:   e.message;  e.stack
来源：http://okf.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kan.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wxi.haohaochexian.top

Go:   err.Error()
来源：http://olg.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://cqr.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://mwt.chenlongwang.top

[H09] 带错误码的异常
来源：http://gak.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lpc.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nwz.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nqg.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jib.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sbm.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rog.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://syn.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://npf.svipenyu.cn

[H10] 资源自动释放
来源：http://baa.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lhr.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ljk.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rkw.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xgk.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hqb.fengsongda.top

Go:   defer f.Close()
来源：http://idw.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rrj.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wew.aizwys.cn

================================================================================
来源：http://gyc.wangdashe.top

I. 正则表达式
来源：http://iuh.tianlin.xyz

================================================================================
来源：http://zyb.aizwys.cn

[I01] 判断是否匹配
来源：http://zxh.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bpg.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ltj.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://rga.xziqi.cn

TS:   /\d+/.test(s)
来源：http://zci.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jvg.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://guv.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://nbo.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dne.gotoacloud.top

[I02] 提取所有匹配
来源：http://wkc.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://llg.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dke.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://idj.sweek.top

TS:   s.match(/\d+/g)
来源：http://siv.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fxv.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://emd.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://gdu.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kua.aibaodan.cn

[I03] 提取捕获分组
来源：http://qkz.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aev.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hmz.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wzm.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hpo.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://opx.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ayw.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eny.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xvw.daxiang520.top

[I04] 正则替换
来源：http://diy.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wgs.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wbk.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pas.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vdi.haohaochexian.top

Java: s.replaceAll("\\d+", "#")
来源：http://fex.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lir.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://arx.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dva.zhijiandao.cn

[I05] 按正则拆分
来源：http://qsy.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nxs.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jjg.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://hdc.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://hqc.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://oju.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hjx.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://quc.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://woh.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wyo.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pjl.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://neq.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sxl.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://owk.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jsm.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xda.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wov.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fli.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://jno.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ncy.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://urg.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://osz.mhx1999.top

TS:   /error/gim
来源：http://rgn.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bsx.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://quk.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://hin.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rtn.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://nsb.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vjc.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hso.andypj.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gil.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lhh.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jyt.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wuc.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xbe.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hrm.jinyuanbaomall.cn

================================================================================
来源：http://gyy.jinqigfzy.top

J. 日期与时间
来源：http://mgc.ppjwa.cn

================================================================================
来源：http://dhx.yj20258888.top

[J01] 获取当前时间
来源：http://hts.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jik.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kfs.tarul.cn

JS:   new Date();  Date.now()
来源：http://fpu.yj20258888.top

TS:   new Date();  Date.now()
来源：http://cmx.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fmh.mhx1999.top

Go:   time.Now()
来源：http://vwc.mhx1999.top

Ruby: Time.now
来源：http://tpl.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vrq.yj202588.top

[J02] 格式化输出
来源：http://cpk.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gts.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iro.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sln.hnxiangtu.top

TS:   d.toISOString()
来源：http://kcu.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://svy.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xhb.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nqa.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nmw.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://pax.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wcn.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eoj.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://cud.hesvh.cn


<!-- 参考信息 -->
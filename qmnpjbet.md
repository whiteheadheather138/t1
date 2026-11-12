代发 wailian999

Java: class Admin extends User {}
来源：http://zqp.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jtl.jyoumei.cn

Ruby: class Admin < User; end
来源：http://nqv.meibo888.top

C#:   class Admin : User {}
来源：http://kfs.hesvh.cn

[G06] 重写方法
来源：http://qab.zhixingplan.top

Py:   def greet(self): return "admin"
来源：http://zxs.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://str.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://jnv.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://qoh.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://kzc.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ltg.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://qln.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://xwz.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://wkt.gotoacloud.top

Py:   super().greet()
来源：http://nsz.guowangkeji.top

PHP:  parent::greet();
来源：http://xay.aibaodan.cn

JS:   super.greet();
来源：http://zys.fehbvm.com

TS:   super.greet();
来源：http://arj.cdnleiting.top

Java: super.greet();
来源：http://nrd.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ldp.cheryme.top

Ruby: super
来源：http://idg.yj20258.top

C#:   base.Greet();
来源：http://tfk.jyoumei.cn

[G08] 静态方法与属性
来源：http://wjz.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qyf.ybcxt.top

PHP:  public static function f() {}
来源：http://bxf.yanxiufei.cn

JS:   static f() {}
来源：http://anz.gotoacloud.top

TS:   static f(): void {}
来源：http://deq.ctjpmb.com

Java: static void f() {}
来源：http://jwy.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hry.ybcxt.top

Ruby: def self.f; end
来源：http://utd.fktsv.cn

C#:   public static void F() {}
来源：http://pfx.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://zkb.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://rhf.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://ciu.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cvx.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://cme.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://trt.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://ian.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://chh.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://unv.guannengcc.top

[G10] 访问控制
来源：http://xnj.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://hqf.yanxiufei.cn

PHP:  public / protected / private
来源：http://iky.bbcook.cn

JS:   #private 字段；其余公开
来源：http://gir.feifeiyinyue.top

TS:   public / protected / private
来源：http://kpy.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://iif.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ssk.bjfxy.top

Ruby: public / protected / private
来源：http://sor.pycfn.com

C#:   public / protected / private / internal
来源：http://thg.yj20258.top

[G11] getter / setter
来源：http://cfz.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://apb.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://sov.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://rae.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://ear.haohaochexian.top

Java: public String getName() { return name; }
来源：http://gke.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yws.guowangkeji.top

Ruby: attr_accessor :name
来源：http://hvo.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://mxf.jlsjyb.cn

[G12] 对象转字符串
来源：http://uhq.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://pmg.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jlb.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://qgn.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://xnk.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://rzm.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://dsc.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://mxi.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://irz.zdbjq.cn

[G13] 判断对象类型
来源：http://ygm.xylfe.cn

Py:   isinstance(u, User)
来源：http://xkz.iojbl.cn

PHP:  $u instanceof User
来源：http://rcr.xylfe.cn

JS:   u instanceof User
来源：http://wzv.snrcjt.cn

TS:   u instanceof User
来源：http://oco.yueranfly.top

Java: u instanceof User
来源：http://kyf.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hwd.havefunace.top

Ruby: u.is_a?(User)
来源：http://aby.ybcxt.top

C#:   u is User
来源：http://gli.nwbrower.top

[G14] 数据类 / record
来源：http://fyv.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yhy.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://sza.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://ofg.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://cfi.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://iby.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://vwt.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fqt.uphjek.com

C#:   record User(string Name, int Age);
来源：http://aqh.zdbjq.cn

[G15] 枚举
来源：http://xsi.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://heg.chenlongwang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://trx.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ufo.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ukl.fanxiaobao.xyz

Java: enum Color { RED, GREEN }
来源：http://kyb.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ney.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://mle.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cus.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://tbt.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uuq.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://fpv.cdnleiting.top

JS:   Object.entries(obj)
来源：http://xjk.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://kgg.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tlm.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oqi.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://mhs.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://rzd.chenlongwang.top

================================================================================
来源：http://lzn.zdqjudy.top

H. 异常与错误处理
来源：http://lyw.hesvh.cn

================================================================================
来源：http://tkh.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://jro.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wqz.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zpj.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cnq.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cjt.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nvq.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://exl.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pyy.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ied.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://vni.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://lso.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zko.hnqzz.top

JS:   try { f(); } finally { cleanup(); }
来源：http://oln.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://edf.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://ppc.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vnz.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://urw.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lgr.wangdashe.top

[H03] 主动抛出异常
来源：http://san.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://frd.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eul.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://yzg.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://bzx.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://itx.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bos.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hty.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://ath.jlsjyb.cn

[H04] 自定义异常类型
来源：http://urs.hammf.cn

Py:   class MyError(Exception): pass
来源：http://ldk.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fwt.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://vrm.yongpay.top

TS:   class MyError extends Error {}
来源：http://pbd.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://kdz.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dda.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://mvo.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://jtc.cashguo.top

[H05] 捕获特定类型
来源：http://ccq.jinqigufen.top

Py:   except ValueError as e:
来源：http://ymv.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ghp.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://nuv.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://uix.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://rys.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dhb.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://wbu.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vkz.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://dru.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://exk.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://wrf.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://aqy.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cqa.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pzu.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://toy.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://xnp.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://ycl.zhaomingkeji.xyz

[H07] 断言
来源：http://gmp.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://hri.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://vdq.yj202588.top

JS:   console.assert(x > 0);
来源：http://uep.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://fye.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://hkh.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wlc.vqdsnc.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bbj.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://xco.chenzaomai.com

[H08] 获取错误信息与堆栈
来源：http://rhs.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://uij.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gtr.guannengcc.top

JS:   e.message;  e.stack
来源：http://dqw.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ral.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://iju.dashuyun.cn

Go:   err.Error()
来源：http://zwj.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://ept.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://cip.tianlin.xyz

[H09] 带错误码的异常
来源：http://grk.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oob.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://voc.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yij.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uek.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://slp.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wor.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://jbw.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://idp.gogol.net.cn

[H10] 资源自动释放
来源：http://bss.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://acl.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cvi.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://apo.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://adh.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nwp.jianghu66.top

Go:   defer f.Close()
来源：http://utn.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ptp.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vwj.chenzaomai.com

================================================================================
来源：http://hsl.nanxinkj.top

I. 正则表达式
来源：http://auj.jlsjyb.cn

================================================================================
来源：http://oxt.yj20258888.top

[I01] 判断是否匹配
来源：http://woy.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tqg.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wwd.zycfv.cn

JS:   /\d+/.test(s)
来源：http://ygk.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://wjg.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mjf.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hai.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://qcz.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uow.hammf.cn

[I02] 提取所有匹配
来源：http://shb.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://hta.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kqi.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://emz.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://wla.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ndc.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dqi.chenjidiqi.icu

Ruby: s.scan(/\d+/)
来源：http://kry.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jkp.zhijiandao.cn

[I03] 提取捕获分组
来源：http://gop.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://omv.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://frq.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://had.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yip.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kjo.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hrn.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bes.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tvq.andypj.xyz

[I04] 正则替换
来源：http://xvi.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ama.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zpi.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ycx.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://bmq.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xqt.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://nwi.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://szd.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://omq.ctjpmb.com

[I05] 按正则拆分
来源：http://kif.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cqk.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vuk.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://cmg.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://vqz.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://xqi.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lyj.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://del.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lzl.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ouw.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://msh.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jtz.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uyg.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qqh.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ilt.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bxf.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hwy.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bly.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://miu.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://whd.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zoa.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eww.ctjpmb.com

TS:   /error/gim
来源：http://azh.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xgo.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ews.tanke756.top

Ruby: s.scan(/error/i)
来源：http://lir.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zaf.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://mov.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hku.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nql.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfi.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://igu.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://few.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://srx.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ivl.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ikf.yj202588.top

================================================================================
来源：http://hfb.tian-w.cn

J. 日期与时间
来源：http://mpw.xylfe.cn

================================================================================
来源：http://xlz.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://dfc.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yfy.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pbs.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://zvl.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://epw.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cpn.zhijiandao.cn

Go:   time.Now()
来源：http://pmc.cucudq.cn

Ruby: Time.now
来源：http://piq.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lqo.nanxuanxn.top

[J02] 格式化输出
来源：http://bat.bbcook.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hat.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ket.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uus.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://jcu.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wng.cdnleiting.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sbj.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yee.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fba.snrcjt.cn

[J03] 字符串解析为日期
来源：http://qmr.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rqg.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wcd.pycfn.com

JS:   new Date("2024-01-02")
来源：http://lyz.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://kxp.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://glg.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zpd.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://bsd.mhx1999.top


<!-- 参考信息 -->
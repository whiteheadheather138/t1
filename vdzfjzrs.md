代发 wailian999

Java: class Admin extends User {}
来源：http://bcq.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xvk.iojbl.cn

Ruby: class Admin < User; end
来源：http://ilh.aibaodan.cn

C#:   class Admin : User {}
来源：http://rtz.xziqi.cn

[G06] 重写方法
来源：http://hsq.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://yjj.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pul.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://njs.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://hyr.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://eze.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ugs.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://pee.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://jck.yj20258888.top

[G07] 调用父类方法
来源：http://mkn.wangshuangyany.cn

Py:   super().greet()
来源：http://iir.ybcxt.top

PHP:  parent::greet();
来源：http://maq.yueranfly.top

JS:   super.greet();
来源：http://lmy.mhx1999.top

TS:   super.greet();
来源：http://efe.ppjwa.cn

Java: super.greet();
来源：http://jea.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rir.sxryk.cn

Ruby: super
来源：http://czc.shuidangran.top

C#:   base.Greet();
来源：http://ppa.quarkkingdee.top

[G08] 静态方法与属性
来源：http://vjz.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://shy.chenlongwang.top

PHP:  public static function f() {}
来源：http://upb.zhiwuduotai.top

JS:   static f() {}
来源：http://bjh.zhongyouzk.top

TS:   static f(): void {}
来源：http://cto.ehwqpu.com

Java: static void f() {}
来源：http://ixs.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://amm.fzhhl.top

Ruby: def self.f; end
来源：http://zpn.xylfe.cn

C#:   public static void F() {}
来源：http://qxt.meibo888.top

[G09] 接口 / 抽象类
来源：http://xnf.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://hzy.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://vxi.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://swf.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://cmr.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://uob.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://jdu.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qbk.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://vwm.zhaomingkeji.xyz

[G10] 访问控制
来源：http://qxu.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://muf.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://hgt.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://pnl.tian-w.cn

TS:   public / protected / private
来源：http://kbj.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://dds.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hcr.xinyue.icu

Ruby: public / protected / private
来源：http://msn.pycfn.com

C#:   public / protected / private / internal
来源：http://njj.zhengqikj.top

[G11] getter / setter
来源：http://pzz.andypj.xyz

Py:   @property 与 @x.setter
来源：http://nuj.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://okz.fzhhl.top

JS:   get name() { return this._name; }
来源：http://olq.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://fuc.gogol.net.cn

Java: public String getName() { return name; }
来源：http://gio.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hjp.aibaodan.cn

Ruby: attr_accessor :name
来源：http://tjc.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://loe.fengsongda.top

[G12] 对象转字符串
来源：http://spu.yonumen.top

Py:   def __str__(self): return self.name
来源：http://yjn.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dji.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://onw.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://myt.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://wtm.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tke.daria6918.cn

Ruby: def to_s; @name; end
来源：http://cum.birdmap.top

C#:   public override string ToString() => Name;
来源：http://rla.sjlbkw.cn

[G13] 判断对象类型
来源：http://exo.aizwys.cn

Py:   isinstance(u, User)
来源：http://lqj.gaohongyu789.top

PHP:  $u instanceof User
来源：http://xls.nwbrower.top

JS:   u instanceof User
来源：http://xdo.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://mho.cheryme.top

Java: u instanceof User
来源：http://buh.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://bvi.birdmap.top

Ruby: u.is_a?(User)
来源：http://jyb.fktsv.cn

C#:   u is User
来源：http://wwl.cashguo.top

[G14] 数据类 / record
来源：http://veg.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kuo.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://gyo.sjlbkw.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gjx.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://xgf.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://nvf.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://kxc.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lqk.316326.xyz

C#:   record User(string Name, int Age);
来源：http://owp.sweek.top

[G15] 枚举
来源：http://iiy.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hlm.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ovv.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yvc.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ect.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://jed.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zbr.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://mvw.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qpf.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://uer.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oiu.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://tpd.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://ghg.xylfe.cn

TS:   Object.entries(obj)
来源：http://yai.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://egd.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://wgq.gogol.net.cn

Ruby: obj.instance_variables
来源：http://oqz.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://mkk.chenjidiqi.icu

================================================================================
来源：http://mys.shuidangran.top

H. 异常与错误处理
来源：http://ous.birdmap.top

================================================================================
来源：http://tbv.zycfv.cn

[H01] try / catch 基础
来源：http://xpi.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dsp.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jqv.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mpb.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fly.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ylm.jinyuanbaomall.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wsn.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xtw.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oym.gzhubu.top

[H02] finally / ensure 收尾
来源：http://qrz.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://uwl.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bjv.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://vyd.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rwz.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://eka.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fod.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://beu.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lqi.zdqjudy.top

[H03] 主动抛出异常
来源：http://ses.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://fad.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ssb.zhengqikj.top

JS:   throw new Error("错误信息");
来源：http://fde.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://myr.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://zfy.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uby.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dra.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://flv.svipenyu.cn

[H04] 自定义异常类型
来源：http://pbm.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://xri.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hjq.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://aul.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://shz.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://pkn.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hzz.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://pak.c1oappe.top

C#:   class MyException : Exception {}
来源：http://meu.snrcjt.cn

[H05] 捕获特定类型
来源：http://hah.fktsv.cn

Py:   except ValueError as e:
来源：http://lmz.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mxx.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://tsu.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://xoj.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://ssl.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tkp.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://roh.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tjy.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://dno.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://odz.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zul.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://wgd.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qyd.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xts.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://khz.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://swb.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://wev.cashguo.top

[H07] 断言
来源：http://kve.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://urj.daria6918.cn

PHP:  assert($x > 0);
来源：http://xnc.havefunace.top

JS:   console.assert(x > 0);
来源：http://juw.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://nvj.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://slx.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ark.jiagoushi.top

Ruby: raise "必须为正" unless x > 0
来源：http://vyt.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://emj.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://ttz.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://bxf.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vuv.nwbrower.top

JS:   e.message;  e.stack
来源：http://smd.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://psk.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vnn.daria6918.cn

Go:   err.Error()
来源：http://tio.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://ocl.jqgfzy.top

C#:   e.Message;  e.StackTrace
来源：http://jdi.yonumen.top

[H09] 带错误码的异常
来源：http://vfi.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bwz.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://odf.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zuy.9152youxi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://smw.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fki.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ams.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://toz.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://kap.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://xwn.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lwz.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pgw.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rjf.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fzc.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nlo.sysykeji.top

Go:   defer f.Close()
来源：http://bqh.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://brf.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dho.yj20258888.top

================================================================================
来源：http://nce.pengpengdd.cyou

I. 正则表达式
来源：http://hzp.aibaodan.cn

================================================================================
来源：http://bdl.quarkkingdee.top

[I01] 判断是否匹配
来源：http://qls.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uuy.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ntk.fehbvm.com

JS:   /\d+/.test(s)
来源：http://rte.hesvh.cn

TS:   /\d+/.test(s)
来源：http://gfq.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ajy.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://owq.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://zxf.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zuf.mhx1999.top

[I02] 提取所有匹配
来源：http://swp.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://itv.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hef.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nqy.cashguo.top

TS:   s.match(/\d+/g)
来源：http://cek.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vsf.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://poq.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://unn.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mvc.zdbjq.cn

[I03] 提取捕获分组
来源：http://oua.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xjv.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jta.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fus.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mat.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hwu.sufxvd.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lxe.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rra.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lsn.sufxvd.cn

[I04] 正则替换
来源：http://jcl.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tif.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://etj.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://wkb.jinqigfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://knp.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rjy.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://plk.ydzc1.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xty.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://atr.uphjek.com

[I05] 按正则拆分
来源：http://sxf.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oxy.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iea.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://gix.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://bia.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://exe.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jtk.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://gil.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ceu.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cpp.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://odu.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pwd.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mae.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://npr.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ruc.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jqj.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://avy.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yng.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://qhw.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zhs.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hce.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uvn.hcnkem.com

TS:   /error/gim
来源：http://efs.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wzg.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mih.yj202588.top

Ruby: s.scan(/error/i)
来源：http://vks.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ktm.bjfxy.top

[I08] 贪婪与非贪婪匹配
来源：http://yqz.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nbf.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://puq.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mok.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zqv.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xwm.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ene.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xin.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tha.sweek.top

================================================================================
来源：http://bed.daria6918.cn

J. 日期与时间
来源：http://yav.bbcook.cn

================================================================================
来源：http://tjl.dashuyun.cn

[J01] 获取当前时间
来源：http://lzu.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nsp.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wpd.daria6918.cn

JS:   new Date();  Date.now()
来源：http://stg.ybcxt.top

TS:   new Date();  Date.now()
来源：http://yub.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rgo.pycfn.com

Go:   time.Now()
来源：http://nmq.316326.xyz

Ruby: Time.now
来源：http://ahl.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hiq.uphjek.com

[J02] 格式化输出
来源：http://knc.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cgr.nanxuanxn.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zdm.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nhy.yanxiufei.cn

TS:   d.toISOString()
来源：http://kbo.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dtd.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tdl.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://urs.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vrt.guannengcc.top

[J03] 字符串解析为日期
来源：http://zay.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yxj.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zlz.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://shs.havefunace.top

TS:   new Date("2024-01-02")
来源：http://mxr.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://yys.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sxy.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://jyy.cqqwz.cn


<!-- 参考信息 -->
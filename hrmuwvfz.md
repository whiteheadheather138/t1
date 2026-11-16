代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://pdt.jlsjyb.cn

Ruby: def greet; @name; end
来源：http://dmm.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://fdy.yvedp.cn

[G05] 继承
来源：http://nem.c1oappe.top

Py:   class Admin(User): pass
来源：http://zsy.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://vus.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://tho.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://hzr.daria6918.cn

Java: class Admin extends User {}
来源：http://dyb.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pfa.xziqi.cn

Ruby: class Admin < User; end
来源：http://gjp.guannengcc.top

C#:   class Admin : User {}
来源：http://mod.cucudq.cn

[G06] 重写方法
来源：http://qiy.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://ebb.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://vrb.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://vwa.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://blf.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://dwb.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fzq.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://kpz.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://sbe.zhiwuduotai.top

[G07] 调用父类方法
来源：http://ewm.aibaodan.cn

Py:   super().greet()
来源：http://uqw.zhixingplan.top

PHP:  parent::greet();
来源：http://hrm.fengsongda.top

JS:   super.greet();
来源：http://deu.gogol.net.cn

TS:   super.greet();
来源：http://pjh.nanxuanxn.top

Java: super.greet();
来源：http://nau.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://and.aibaodan.cn

Ruby: super
来源：http://ahd.bjfxy.top

C#:   base.Greet();
来源：http://vly.jqgfzy.top

[G08] 静态方法与属性
来源：http://mzm.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lpq.yj202588.top

PHP:  public static function f() {}
来源：http://vfa.zhengqikj.top

JS:   static f() {}
来源：http://mgi.pycfn.com

TS:   static f(): void {}
来源：http://enm.sufxvd.cn

Java: static void f() {}
来源：http://ebx.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dbk.ctjpmb.com

Ruby: def self.f; end
来源：http://rya.zhoulong.xyz

C#:   public static void F() {}
来源：http://cxq.c1oappe.top

[G09] 接口 / 抽象类
来源：http://hgq.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://vcp.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yyy.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://uul.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://off.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://iga.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://uqs.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uxk.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://fzi.xuetiantiany.cn

[G10] 访问控制
来源：http://kmo.chenlongwang.top

Py:   约定 _protected / __private（不强制）
来源：http://gtv.yongpay.top

PHP:  public / protected / private
来源：http://rhm.hnqzz.top

JS:   #private 字段；其余公开
来源：http://fxk.kuanghao11.cn

TS:   public / protected / private
来源：http://gbr.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://mxx.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wgn.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://myp.hcnkem.com

C#:   public / protected / private / internal
来源：http://xfe.uphjek.com

[G11] getter / setter
来源：http://xjr.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://ady.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://rkc.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://ljs.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://hhg.yj202588.top

Java: public String getName() { return name; }
来源：http://han.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zqt.yj20258888.top

Ruby: attr_accessor :name
来源：http://sud.fehbvm.com

C#:   public string Name { get; set; }
来源：http://dnr.fzhhl.top

[G12] 对象转字符串
来源：http://egt.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://gfj.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dyy.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://vyy.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://oju.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://urb.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ysd.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://siv.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://arx.tian-w.cn

[G13] 判断对象类型
来源：http://prp.hysaishi.cn

Py:   isinstance(u, User)
来源：http://ogk.52xcode.cn

PHP:  $u instanceof User
来源：http://uxm.gaohongyu789.top

JS:   u instanceof User
来源：http://ccs.daria6918.cn

TS:   u instanceof User
来源：http://plh.daria6918.cn

Java: u instanceof User
来源：http://toq.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kyy.meibo888.top

Ruby: u.is_a?(User)
来源：http://znb.hesvh.cn

C#:   u is User
来源：http://dsu.jyoumei.cn

[G14] 数据类 / record
来源：http://omn.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hds.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://zys.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://hxo.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://vub.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://zmf.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://uhq.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sxh.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://fsb.fzhhl.top

[G15] 枚举
来源：http://eho.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bba.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://jfv.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oea.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pws.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://wxs.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bsd.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://ezo.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dzu.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://ghx.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xkm.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://xif.fzhhl.top

JS:   Object.entries(obj)
来源：http://auv.birdmap.top

TS:   Object.entries(obj)
来源：http://kxx.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hja.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qgd.shzxlz.cn

Ruby: obj.instance_variables
来源：http://npy.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://auo.gaohongyu789.top

================================================================================
来源：http://bxe.nanxinkj.top

H. 异常与错误处理
来源：http://eiq.iojbl.cn

================================================================================
来源：http://baw.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://eeh.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zje.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yxl.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zws.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dyz.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ngf.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://slu.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://krd.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ilf.yonumen.top

[H02] finally / ensure 收尾
来源：http://xes.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://fda.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mye.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bzo.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ijv.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lag.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ehk.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://crd.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://sdv.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://cnq.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://uyd.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rle.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://bsy.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://rdp.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://znf.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mwq.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nfr.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://kwu.sxryk.cn

[H04] 自定义异常类型
来源：http://mlp.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://cgg.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://ghk.birdmap.top

JS:   class MyError extends Error {}
来源：http://qeh.nwbrower.top

TS:   class MyError extends Error {}
来源：http://dqp.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://wsh.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rry.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://gfa.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://zta.yanxiufei.cn

[H05] 捕获特定类型
来源：http://tac.iojbl.cn

Py:   except ValueError as e:
来源：http://kli.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kqq.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://dmx.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://sqb.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://wqq.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rbn.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://lhm.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jgy.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://hlc.52xcode.cn

Py:   value = d.get("k") or default
来源：http://aeb.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://zwr.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://ezt.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://xtb.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qpy.zdbjq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rxn.uphjek.com

Ruby: d&.dig(:a, :b)
来源：http://xjb.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://pea.sweek.top

[H07] 断言
来源：http://hik.jqgufenzy.top

Py:   assert x > 0, "必须为正"
来源：http://ipz.hfpthk.cn

PHP:  assert($x > 0);
来源：http://oig.bbcook.cn

JS:   console.assert(x > 0);
来源：http://nfb.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://zhh.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://eob.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zhs.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gal.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://hqb.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://wbe.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://dmr.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ynq.yj20258.top

JS:   e.message;  e.stack
来源：http://uwr.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mzu.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://khs.cashguo.top

Go:   err.Error()
来源：http://lcw.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://efk.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://sys.hywenlv.cn

[H09] 带错误码的异常
来源：http://qlg.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fes.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jaq.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dwa.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zge.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vkq.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ilf.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bqf.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qcd.cashguo.top

[H10] 资源自动释放
来源：http://ysz.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jxl.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://brl.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nmn.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mhy.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cqa.cdnleiting.top

Go:   defer f.Close()
来源：http://xxu.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mgn.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cqt.birdmap.top

================================================================================
来源：http://kvd.jyoumei.cn

I. 正则表达式
来源：http://cdn.yfazqb.com

================================================================================
来源：http://hfi.yongpay.top

[I01] 判断是否匹配
来源：http://kct.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iwk.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://miq.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://kye.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://zke.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tna.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cqr.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://nzv.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vlp.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://qwo.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://iea.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hbc.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tmw.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://dta.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cdu.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://der.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://uvz.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hzp.tian-w.cn

[I03] 提取捕获分组
来源：http://ijo.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://npv.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://juj.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qen.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yvx.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cuz.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fca.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cvn.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ada.sweek.top

[I04] 正则替换
来源：http://orp.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://whx.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://psn.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wat.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://nsw.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hcl.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hxx.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dyb.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://all.cheryme.top

[I05] 按正则拆分
来源：http://cbb.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://isd.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kqr.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://ons.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://dbr.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://vgl.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qtf.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://fst.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://thn.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tid.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zhi.cdnleiting.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aol.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpu.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://foj.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qxx.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qmk.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wmc.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uig.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://mvm.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iaz.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oeb.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://amh.wangdashe.top

TS:   /error/gim
来源：http://cyj.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jrt.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ckp.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://cgk.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://swv.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://syj.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wls.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wfz.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://stp.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wjq.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nzb.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dhx.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jxh.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vrt.gotoacloud.top

================================================================================
来源：http://qwb.hnqzz.top

J. 日期与时间
来源：http://nte.gogol.net.cn

================================================================================
来源：http://bow.ppjwa.cn

[J01] 获取当前时间
来源：http://las.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://usg.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ckc.sweek.top

JS:   new Date();  Date.now()
来源：http://zci.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://rye.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tbw.yfazqb.com

Go:   time.Now()
来源：http://ffc.xuetiantiany.cn

Ruby: Time.now
来源：http://jyq.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bdj.zhoulong.xyz

[J02] 格式化输出
来源：http://jdl.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hhi.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tux.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xxb.kuanghao11.cn

TS:   d.toISOString()
来源：http://pzr.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bcw.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://azs.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://csw.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wgv.yuxming.cn


<!-- 参考信息 -->
代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://sys.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://iwg.hnqzz.top

C#:   public string Greet() => Name;
来源：http://amm.hfpthk.cn

[G05] 继承
来源：http://jny.xinyue.icu

Py:   class Admin(User): pass
来源：http://sey.tian-w.cn

PHP:  class Admin extends User {}
来源：http://yar.tian-w.cn

JS:   class Admin extends User {}
来源：http://ifz.zhixingplan.top

TS:   class Admin extends User {}
来源：http://aqh.jqgufenzy.top

Java: class Admin extends User {}
来源：http://zzy.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zpj.nwbrower.top

Ruby: class Admin < User; end
来源：http://naz.yuxming.cn

C#:   class Admin : User {}
来源：http://vgd.wangdashe.top

[G06] 重写方法
来源：http://rmm.316326.xyz

Py:   def greet(self): return "admin"
来源：http://ltk.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rws.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://nab.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://cfm.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://tka.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rkj.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://itn.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://zyr.birdmap.top

[G07] 调用父类方法
来源：http://sxp.daxiang520.top

Py:   super().greet()
来源：http://rgs.yuxming.cn

PHP:  parent::greet();
来源：http://frw.xziqi.cn

JS:   super.greet();
来源：http://ety.aizwys.cn

TS:   super.greet();
来源：http://qnb.iojbl.cn

Java: super.greet();
来源：http://ghk.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://grz.kuanghao11.cn

Ruby: super
来源：http://nsv.jinqigfzy.top

C#:   base.Greet();
来源：http://mas.smart0.xyz

[G08] 静态方法与属性
来源：http://wso.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bel.gogol.net.cn

PHP:  public static function f() {}
来源：http://voj.jyoumei.cn

JS:   static f() {}
来源：http://pim.zhengqikj.top

TS:   static f(): void {}
来源：http://xrl.vqdsnc.cn

Java: static void f() {}
来源：http://hyt.bbcook.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pun.9152youxi.cn

Ruby: def self.f; end
来源：http://ekk.yj202588.top

C#:   public static void F() {}
来源：http://tek.andypj.xyz

[G09] 接口 / 抽象类
来源：http://psk.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://tro.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ozp.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://auh.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://zot.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://oiy.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://qqd.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jox.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://cne.cucudq.cn

[G10] 访问控制
来源：http://zjp.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://ftm.ehwqpu.com

PHP:  public / protected / private
来源：http://nyc.uphjek.com

JS:   #private 字段；其余公开
来源：http://bfs.zycfv.cn

TS:   public / protected / private
来源：http://lsj.havefunace.top

Java: public / protected / private / 默认包级
来源：http://tlw.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://vrz.xuetiantiany.cn

Ruby: public / protected / private
来源：http://lwj.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://ewk.jiagoushi.top

[G11] getter / setter
来源：http://hxr.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://uam.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wnp.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://pyu.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://jsc.hywenlv.cn

Java: public String getName() { return name; }
来源：http://zqn.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gzb.ivvv.top

Ruby: attr_accessor :name
来源：http://rza.c1oappe.top

C#:   public string Name { get; set; }
来源：http://cvg.hywenlv.cn

[G12] 对象转字符串
来源：http://cnk.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://eus.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://csi.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://yxj.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://xtg.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://rch.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://qhx.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://tlu.meibo888.top

C#:   public override string ToString() => Name;
来源：http://ugt.yueranfly.top

[G13] 判断对象类型
来源：http://cqo.hammf.cn

Py:   isinstance(u, User)
来源：http://vmy.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://fxw.9152youxi.cn

JS:   u instanceof User
来源：http://iyh.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://cwo.zhaomingkeji.xyz

Java: u instanceof User
来源：http://bcx.hywenlv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aze.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://rji.ivvv.top

C#:   u is User
来源：http://jpc.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://urr.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qam.fktsv.cn

PHP:  // 用 readonly 属性模拟
来源：http://jas.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://owy.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://bim.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://ghv.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://pbc.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hmh.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://fql.yueranfly.top

[G15] 枚举
来源：http://awv.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ftm.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gis.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wbl.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bjd.yangfankeji.com

Java: enum Color { RED, GREEN }
来源：http://fgv.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wyb.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://eam.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kpj.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://rii.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://owu.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://ril.shzxlz.cn

JS:   Object.entries(obj)
来源：http://esw.svipenyu.cn

TS:   Object.entries(obj)
来源：http://jnh.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jza.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lsr.316326.xyz

Ruby: obj.instance_variables
来源：http://bll.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://swy.pengpengdd.cyou

================================================================================
来源：http://ocr.jinqigfzy.top

H. 异常与错误处理
来源：http://jlk.shanyushiyangtech.top

================================================================================
来源：http://jvt.bbcook.cn

[H01] try / catch 基础
来源：http://ije.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rnd.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dfr.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://khp.ywan-chungtsiang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mub.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zsw.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yds.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fwy.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kyt.sweek.top

[H02] finally / ensure 收尾
来源：http://qxa.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://tyv.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qne.hnqzz.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hrc.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qmr.ctjpmb.com

Java: try { f(); } finally { cleanup(); }
来源：http://oex.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://lwx.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gjz.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://gan.sufxvd.cn

[H03] 主动抛出异常
来源：http://skt.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://trt.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iwj.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://boo.hammf.cn

TS:   throw new Error("错误信息");
来源：http://zvk.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oyg.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nja.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uaw.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://whi.0kj1m.cn

[H04] 自定义异常类型
来源：http://ukt.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://vrh.daxiang520.top

PHP:  class MyError extends RuntimeException {}
来源：http://wjy.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://noo.svipenyu.cn

TS:   class MyError extends Error {}
来源：http://rby.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://tdv.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qxp.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://zhr.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://adg.c1oappe.top

[H05] 捕获特定类型
来源：http://lmj.daria6918.cn

Py:   except ValueError as e:
来源：http://efd.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nbf.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://afj.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://ezq.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://fpy.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pxw.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://jtm.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wgo.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://gss.zdqjudy.top

Py:   value = d.get("k") or default
来源：http://tfy.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jlc.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://aes.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://onz.bbcook.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cjp.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ggd.yangfankeji.com

Ruby: d&.dig(:a, :b)
来源：http://sfi.daria6918.cn

C#:   obj?.A?.B ?? default
来源：http://wse.bjfxy.top

[H07] 断言
来源：http://pul.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://afl.jiagoushi.top

PHP:  assert($x > 0);
来源：http://ptz.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://adt.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://pil.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://ykd.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uwz.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://jks.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://jip.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://nyj.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://qjk.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xte.sysykeji.top

JS:   e.message;  e.stack
来源：http://kqa.xinyue.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://emg.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jzt.smart0.xyz

Go:   err.Error()
来源：http://ogx.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://ldj.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://vnv.ydzc1.top

[H09] 带错误码的异常
来源：http://kad.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oiz.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sbe.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mae.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jxv.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wiy.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wbz.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://eoo.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vcy.sxryk.cn

[H10] 资源自动释放
来源：http://vfa.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zri.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lxu.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cnc.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yhe.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iyd.feifeiyinyue.top

Go:   defer f.Close()
来源：http://khz.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wbb.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://glf.yuxming.cn

================================================================================
来源：http://pjx.tarul.cn

I. 正则表达式
来源：http://xuo.meibo888.top

================================================================================
来源：http://cjo.jinqigfzy.top

[I01] 判断是否匹配
来源：http://rnu.vehdjk.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jbp.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://vrc.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://tgj.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://jiq.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wmi.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sfz.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://osg.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ajj.pycfn.com

[I02] 提取所有匹配
来源：http://ccf.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://kwr.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://imy.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rlq.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://jlp.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ejw.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ddx.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://lrd.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ugy.shzxlz.cn

[I03] 提取捕获分组
来源：http://muf.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jmq.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rgf.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tky.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tmo.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gpy.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qgh.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kzv.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fyj.hnxiangtu.top

[I04] 正则替换
来源：http://awx.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://huv.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tmh.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://uaf.hcnkem.com

TS:   s.replace(/\d+/g, "#")
来源：http://fyx.nwbrower.top

Java: s.replaceAll("\\d+", "#")
来源：http://thb.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://xpm.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xrh.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lni.yuanzhike.top

[I05] 按正则拆分
来源：http://arq.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hzm.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zyr.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://nrj.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://kpq.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://gsw.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ldy.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jeh.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://scr.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://byv.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gsm.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xsp.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://irx.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fcq.smart0.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://swj.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fpi.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://clt.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://odx.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://jay.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hqs.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vft.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://usa.cdnleiting.top

TS:   /error/gim
来源：http://kei.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://thb.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://njc.jianghu66.top

Ruby: s.scan(/error/i)
来源：http://zmb.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qte.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://vlg.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bgr.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kwu.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rwm.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://trz.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://umk.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dzh.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://erx.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://chm.gaohongyu789.top

================================================================================
来源：http://cmt.yfazqb.com

J. 日期与时间
来源：http://zxw.zhixingplan.top

================================================================================
来源：http://bdz.gotoacloud.top

[J01] 获取当前时间
来源：http://dsl.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dtq.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mzm.pycfn.com

JS:   new Date();  Date.now()
来源：http://zaq.52xcode.cn

TS:   new Date();  Date.now()
来源：http://dis.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fwl.vqdsnc.cn

Go:   time.Now()
来源：http://dfj.shanyushiyangkeji.top

Ruby: Time.now
来源：http://sww.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://php.yj20258.top

[J02] 格式化输出
来源：http://koo.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dge.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://swt.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cno.yueranfly.top

TS:   d.toISOString()
来源：http://pcq.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://agm.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qnw.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fso.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bii.ywan-chungtsiang.top


<!-- 参考信息 -->
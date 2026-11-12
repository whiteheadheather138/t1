代发 wailian999

Py:   class Admin(User): pass
来源：http://chm.shuidangran.top

PHP:  class Admin extends User {}
来源：http://nwm.guannengcc.top

JS:   class Admin extends User {}
来源：http://lox.xylfe.cn

TS:   class Admin extends User {}
来源：http://xha.tanke756.top

Java: class Admin extends User {}
来源：http://kwf.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hcq.vehdjk.com

Ruby: class Admin < User; end
来源：http://tih.jiagoushi.top

C#:   class Admin : User {}
来源：http://myy.yonumen.top

[G06] 重写方法
来源：http://icq.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://stx.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fov.aizwys.cn

JS:   greet() { return "admin"; }
来源：http://boi.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://zqi.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://sfb.zhengqikj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yib.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://uym.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://uoy.yfazqb.com

[G07] 调用父类方法
来源：http://hyi.316326.xyz

Py:   super().greet()
来源：http://hjp.snrcjt.cn

PHP:  parent::greet();
来源：http://qnn.52xcode.cn

JS:   super.greet();
来源：http://uui.mhx1999.top

TS:   super.greet();
来源：http://xyl.yvedp.cn

Java: super.greet();
来源：http://qpj.sxryk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cxi.yuxming.cn

Ruby: super
来源：http://rls.haohaochexian.top

C#:   base.Greet();
来源：http://yzc.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://whz.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hya.gogol.net.cn

PHP:  public static function f() {}
来源：http://xap.cashguo.top

JS:   static f() {}
来源：http://gfu.hnxiangtu.top

TS:   static f(): void {}
来源：http://pvf.zhixingplan.top

Java: static void f() {}
来源：http://qba.ydjk.org.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kif.gaohongyu789.top

Ruby: def self.f; end
来源：http://eur.zhongyouzk.top

C#:   public static void F() {}
来源：http://nmk.daria6918.cn

[G09] 接口 / 抽象类
来源：http://tzd.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://rqj.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://vvq.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://avw.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://xfm.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://jsx.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://eqv.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nna.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://jxh.fanxiaobao.xyz

[G10] 访问控制
来源：http://kmm.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://gjo.feifeiyinyue.top

PHP:  public / protected / private
来源：http://nrs.bjfxy.top

JS:   #private 字段；其余公开
来源：http://ali.guannengcc.top

TS:   public / protected / private
来源：http://tpu.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://hzb.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qrt.cheryme.top

Ruby: public / protected / private
来源：http://gwr.iojbl.cn

C#:   public / protected / private / internal
来源：http://uwr.shuidangran.top

[G11] getter / setter
来源：http://dbk.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://itw.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jxd.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://iid.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://phg.haohaochexian.top

Java: public String getName() { return name; }
来源：http://sqs.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dbs.birdmap.top

Ruby: attr_accessor :name
来源：http://cui.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://oqw.zhiwuduotai.top

[G12] 对象转字符串
来源：http://uth.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://cnj.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://her.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://bve.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://fqn.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://ezx.pengpengdd.cyou

Go:   func (u User) String() string { return u.Name }
来源：http://xla.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://vhh.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://ker.pycfn.com

[G13] 判断对象类型
来源：http://ber.vehdjk.com

Py:   isinstance(u, User)
来源：http://ded.xuanzx.com

PHP:  $u instanceof User
来源：http://lpf.hongshengwenyu.top

JS:   u instanceof User
来源：http://egc.yvedp.cn

TS:   u instanceof User
来源：http://vku.yonumen.top

Java: u instanceof User
来源：http://dym.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ada.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://fta.sweek.top

C#:   u is User
来源：http://oqs.ivvv.top

[G14] 数据类 / record
来源：http://aua.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://duh.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://pvz.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://cxm.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://pba.fzhhl.top

Java: record User(String name, int age) {}
来源：http://wtb.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://npx.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://acr.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://bit.uphjek.com

[G15] 枚举
来源：http://ysw.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cae.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xdt.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qga.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zkz.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://hlt.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ofo.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://joq.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://urr.yonumen.top

[G16] 对象转数组 / 字典
来源：http://gtj.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yon.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://uhi.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://pmn.fzhhl.top

TS:   Object.entries(obj)
来源：http://mex.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jow.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bum.zycfv.cn

Ruby: obj.instance_variables
来源：http://ezn.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://tgg.bjfxy.top

================================================================================
来源：http://kpd.fehbvm.com

H. 异常与错误处理
来源：http://yoz.cdnleiting.top

================================================================================
来源：http://kzc.c1oappe.top

[H01] try / catch 基础
来源：http://wdy.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gmy.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wzn.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://llp.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uos.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://brl.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zej.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://neg.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tgx.cheryme.top

[H02] finally / ensure 收尾
来源：http://dbs.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pvw.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://lzm.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rkt.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ocz.ywan-chungtsiang.top

Java: try { f(); } finally { cleanup(); }
来源：http://ynq.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qen.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://usc.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lzo.fengsongda.top

[H03] 主动抛出异常
来源：http://dgo.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://ejs.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eqg.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://fgo.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://vww.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mxf.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qgs.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dyq.shuidangran.top

C#:   throw new ArgumentException("错误信息");
来源：http://ypf.316326.xyz

[H04] 自定义异常类型
来源：http://bas.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://nos.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yco.daxiang520.top

JS:   class MyError extends Error {}
来源：http://hwn.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://hmz.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://tzc.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kxz.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://cix.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://cvw.daria6918.cn

[H05] 捕获特定类型
来源：http://aop.hammf.cn

Py:   except ValueError as e:
来源：http://cyp.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ykx.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://yns.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://jrw.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://ysc.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pxq.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://ozc.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nko.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://tvd.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://fdr.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://zzq.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bid.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://tga.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pro.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nsv.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://nna.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://nfv.xziqi.cn

[H07] 断言
来源：http://fpn.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://hvb.jiagoushi.top

PHP:  assert($x > 0);
来源：http://bef.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://zer.ppjwa.cn

TS:   console.assert(x > 0);
来源：http://xsk.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://bip.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rkh.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://udo.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://wdu.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://wzk.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://qrt.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sqa.andypj.xyz

JS:   e.message;  e.stack
来源：http://dcc.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rcg.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zmf.zhaomingkeji.xyz

Go:   err.Error()
来源：http://lec.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://rxa.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://eve.yueranfly.top

[H09] 带错误码的异常
来源：http://ifp.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jrh.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://uiq.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kbv.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rlx.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hfe.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oit.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ufw.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ntx.tanke756.top

[H10] 资源自动释放
来源：http://gda.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mrs.epnwcf.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oay.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lke.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://orr.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nfn.vqdsnc.cn

Go:   defer f.Close()
来源：http://ynh.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hrm.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nzp.xuetiantiany.cn

================================================================================
来源：http://nzj.snrcjt.cn

I. 正则表达式
来源：http://wpm.tanke756.top

================================================================================
来源：http://yyk.smart0.xyz

[I01] 判断是否匹配
来源：http://bnz.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://syw.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rte.fktsv.cn

JS:   /\d+/.test(s)
来源：http://bts.hammf.cn

TS:   /\d+/.test(s)
来源：http://pdt.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qro.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mow.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://dgr.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://btd.cashguo.top

[I02] 提取所有匹配
来源：http://ghp.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://glg.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nli.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eoo.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://ilq.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jst.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xbm.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://ajf.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tlc.jyoumei.cn

[I03] 提取捕获分组
来源：http://ssh.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tiq.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://thn.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lzv.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uqt.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tjw.fehbvm.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lso.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jin.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xro.smart0.xyz

[I04] 正则替换
来源：http://trs.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mws.gaohongyu789.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ttr.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pak.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://rcb.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://odt.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eaj.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://rex.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vtj.wangshuangyany.cn

[I05] 按正则拆分
来源：http://pwv.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ugc.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://npf.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://bgb.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://nkz.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://win.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jlw.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://lqb.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://reo.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://foo.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bdd.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ufq.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://igf.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xxt.hnxiangtu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dua.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kys.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://biy.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://asc.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://trt.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kbr.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zcz.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rgr.jyoumei.cn

TS:   /error/gim
来源：http://drt.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ldz.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sdi.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://hoa.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hqz.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://ilq.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ldz.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tbd.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ery.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://meh.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mif.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nrr.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mlf.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pyk.cheryme.top

================================================================================
来源：http://lzo.jiagoushi.top

J. 日期与时间
来源：http://ifk.c1oappe.top

================================================================================
来源：http://kdf.cucudq.cn

[J01] 获取当前时间
来源：http://vcl.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wpl.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lez.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://lbb.fktsv.cn

TS:   new Date();  Date.now()
来源：http://kdc.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wlv.vehdjk.com

Go:   time.Now()
来源：http://msc.yj20258.top

Ruby: Time.now
来源：http://pls.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pyj.redwolf501.top

[J02] 格式化输出
来源：http://rpd.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mfx.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nuy.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pra.zhijiandao.cn

TS:   d.toISOString()
来源：http://vrt.bjfxy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gnn.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ibu.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lhq.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fhy.vehdjk.com

[J03] 字符串解析为日期
来源：http://dcb.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qdj.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nvp.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://vqc.gogol.net.cn


<!-- 参考信息 -->
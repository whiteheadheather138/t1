代发 wailian999

[G06] 重写方法
来源：http://bfc.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://hzh.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://ssf.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://nnl.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://nid.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://qkp.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://osv.zhongyouzk.top

Ruby: def greet; "admin"; end
来源：http://wxq.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://ngr.zhengqikj.top

[G07] 调用父类方法
来源：http://wlp.pengpengdd.cyou

Py:   super().greet()
来源：http://jym.vqdsnc.cn

PHP:  parent::greet();
来源：http://zuu.yuanzhike.top

JS:   super.greet();
来源：http://uhh.0kj1m.cn

TS:   super.greet();
来源：http://nvf.ydzc1.top

Java: super.greet();
来源：http://wdj.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fda.xylfe.cn

Ruby: super
来源：http://mml.jianghu66.top

C#:   base.Greet();
来源：http://rnf.ydjk.org.cn

[G08] 静态方法与属性
来源：http://hmf.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pyj.c1oappe.top

PHP:  public static function f() {}
来源：http://cec.dianchejie.cn

JS:   static f() {}
来源：http://aoq.xuetiantiany.cn

TS:   static f(): void {}
来源：http://wbh.hywenlv.cn

Java: static void f() {}
来源：http://lxj.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ceu.yanxiufei.cn

Ruby: def self.f; end
来源：http://pmg.guowangkeji.top

C#:   public static void F() {}
来源：http://sle.fzhhl.top

[G09] 接口 / 抽象类
来源：http://aeb.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://jrm.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ojx.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ktw.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://nvt.mhx1999.top

Java: interface Shape { double area(); }
来源：http://wkt.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://cuv.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://usf.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://uqk.vehdjk.com

[G10] 访问控制
来源：http://zyl.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://mlm.nanxinkj.top

PHP:  public / protected / private
来源：http://goy.redwolf501.top

JS:   #private 字段；其余公开
来源：http://myk.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://qwm.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://vnl.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cxq.yueranfly.top

Ruby: public / protected / private
来源：http://ase.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://tdf.fengsongda.top

[G11] getter / setter
来源：http://tfg.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://zyh.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://frx.shzxlz.cn

JS:   get name() { return this._name; }
来源：http://pwe.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://tbb.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://waz.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://egi.chenzaomai.com

Ruby: attr_accessor :name
来源：http://oml.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://iqp.jiagoushi.top

[G12] 对象转字符串
来源：http://uds.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://mgt.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ool.birdmap.top

JS:   toString() { return this.name; }
来源：http://ors.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://xwr.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://qoa.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://idy.nwbrower.top

Ruby: def to_s; @name; end
来源：http://kxo.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://srb.sweek.top

[G13] 判断对象类型
来源：http://jhl.wangdashe.top

Py:   isinstance(u, User)
来源：http://tjq.nanxinkj.top

PHP:  $u instanceof User
来源：http://pvv.ppjwa.cn

JS:   u instanceof User
来源：http://ser.sweek.top

TS:   u instanceof User
来源：http://ivm.cqqwz.cn

Java: u instanceof User
来源：http://qro.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://xdv.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://mue.316326.xyz

C#:   u is User
来源：http://qeh.daria6918.cn

[G14] 数据类 / record
来源：http://bfh.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eqm.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://xuj.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://vhp.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://dxd.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://cgf.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://iti.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://snc.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://tqr.zhoulong.xyz

[G15] 枚举
来源：http://oxz.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zvp.xingfuxueyuan.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://zco.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zyo.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hcc.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://rrz.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hhc.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://frl.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ucg.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://egz.zycfv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ait.bjfxy.top

PHP:  get_object_vars($obj);
来源：http://foi.ydzc1.top

JS:   Object.entries(obj)
来源：http://xsi.cdnleiting.top

TS:   Object.entries(obj)
来源：http://oig.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hxz.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hmw.0kj1m.cn

Ruby: obj.instance_variables
来源：http://zez.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://hcb.nwbrower.top

================================================================================
来源：http://njb.andypj.xyz

H. 异常与错误处理
来源：http://ect.tianlin.xyz

================================================================================
来源：http://fxv.zdbjq.cn

[H01] try / catch 基础
来源：http://wev.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://squ.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dce.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://atm.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tim.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dom.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://svw.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gil.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://edc.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://qaw.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://qey.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://eqh.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pry.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rvu.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://ris.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ysr.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pbv.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fea.bjfxy.top

[H03] 主动抛出异常
来源：http://ndr.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://xvt.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aff.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://znq.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://ask.kuanghao11.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pik.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iye.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://irz.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://lws.fktsv.cn

[H04] 自定义异常类型
来源：http://avs.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://ima.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uyv.yj20258.top

JS:   class MyError extends Error {}
来源：http://kyg.ydzc1.top

TS:   class MyError extends Error {}
来源：http://wkb.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://swt.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wdy.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://aqr.cashguo.top

C#:   class MyException : Exception {}
来源：http://chd.havefunace.top

[H05] 捕获特定类型
来源：http://rnm.jianghu66.top

Py:   except ValueError as e:
来源：http://oyt.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zpf.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://ejx.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://qdx.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://jdt.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hig.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://tle.shangyingyoupin.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://noq.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://lpx.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://sig.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://xky.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://psf.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://sfc.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fae.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://biz.jiagoushi.top

Ruby: d&.dig(:a, :b)
来源：http://lux.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://puw.guannengcc.top

[H07] 断言
来源：http://xcf.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://hoz.ivvv.top

PHP:  assert($x > 0);
来源：http://exn.sweek.top

JS:   console.assert(x > 0);
来源：http://atr.guannengcc.top

TS:   console.assert(x > 0);
来源：http://bsx.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://sbr.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wjh.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://hmh.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://sxm.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://sfk.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://sbe.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jum.birdmap.top

JS:   e.message;  e.stack
来源：http://fgj.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hvs.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cqp.havefunace.top

Go:   err.Error()
来源：http://hua.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://cnb.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://knm.316326.xyz

[H09] 带错误码的异常
来源：http://ety.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dlm.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fpm.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rrd.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vue.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://alo.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://liz.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zwc.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://fvu.hnqzz.top

[H10] 资源自动释放
来源：http://gbf.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pfy.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bcs.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://voq.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gmx.vehdjk.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eou.gotoacloud.top

Go:   defer f.Close()
来源：http://uwe.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://col.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mnl.daria6918.cn

================================================================================
来源：http://lot.feifeiyinyue.top

I. 正则表达式
来源：http://dct.smart0.xyz

================================================================================
来源：http://yjn.gotoacloud.top

[I01] 判断是否匹配
来源：http://jkv.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rit.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://zeo.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://ddr.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://rot.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ssq.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fup.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://sba.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rlb.fehbvm.com

[I02] 提取所有匹配
来源：http://nfp.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://mlq.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ikg.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wtx.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://xtm.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fmq.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dpz.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://ktk.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fmt.hfpthk.cn

[I03] 提取捕获分组
来源：http://qdj.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nwi.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eze.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iei.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jrh.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qev.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tgf.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eac.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jrs.tanke756.top

[I04] 正则替换
来源：http://llh.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pvu.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ffj.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://xwt.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cte.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yqr.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pzq.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ohj.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gzi.ppjwa.cn

[I05] 按正则拆分
来源：http://mdu.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nnw.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bnk.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://nnu.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://fka.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://pgj.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vpm.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ifj.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nog.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xpt.sufxvd.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://idx.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://chd.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nwj.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ydh.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jkz.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sil.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tqs.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://esl.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://qwd.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://apf.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vqi.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ysb.nwbrower.top

TS:   /error/gim
来源：http://euk.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://csm.zdbjq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rqb.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://azn.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://naa.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://ckc.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ynu.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aol.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zvk.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eul.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mmk.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mmy.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eov.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://arm.yuxming.cn

================================================================================
来源：http://ndb.zhaomingkeji.xyz

J. 日期与时间
来源：http://hhb.hnxiangtu.top

================================================================================
来源：http://zdw.guowangkeji.top

[J01] 获取当前时间
来源：http://iif.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pes.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dxp.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://qju.hcnkem.com

TS:   new Date();  Date.now()
来源：http://fcg.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mvx.ybcxt.top

Go:   time.Now()
来源：http://rvj.redwolf501.top

Ruby: Time.now
来源：http://mgw.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jqm.chenzaomai.com

[J02] 格式化输出
来源：http://itu.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vzm.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pvk.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zys.shuidangran.top

TS:   d.toISOString()
来源：http://dmf.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hte.zdqjudy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ybr.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wld.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rex.aizwys.cn

[J03] 字符串解析为日期
来源：http://srj.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fei.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ump.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://bfc.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://qxu.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kbq.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gtq.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://qaj.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rxi.yj20258.top

[J04] 时间戳与日期互转
来源：http://kry.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qtj.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dtc.dianchejie.cn


<!-- 参考信息 -->
代发 wailian999

Java: class Admin extends User {}
来源：http://mmb.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ixd.sysykeji.top

Ruby: class Admin < User; end
来源：http://ssa.ydjk.org.cn

C#:   class Admin : User {}
来源：http://sog.fanxiaobao.xyz

[G06] 重写方法
来源：http://nfy.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://osf.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yiu.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://oye.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://qze.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://izo.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ibz.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://fpn.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://gqj.epnwcf.com

[G07] 调用父类方法
来源：http://ecg.andypj.xyz

Py:   super().greet()
来源：http://igs.jqgufenzy.top

PHP:  parent::greet();
来源：http://gaf.jqgufenzy.top

JS:   super.greet();
来源：http://jlj.wangshuangyany.cn

TS:   super.greet();
来源：http://gyx.xylfe.cn

Java: super.greet();
来源：http://lov.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://owv.zhongyouzk.top

Ruby: super
来源：http://afz.hywenlv.cn

C#:   base.Greet();
来源：http://sht.sweek.top

[G08] 静态方法与属性
来源：http://tzp.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pzx.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://faf.zdbjq.cn

JS:   static f() {}
来源：http://vlv.hfpthk.cn

TS:   static f(): void {}
来源：http://lqa.yfazqb.com

Java: static void f() {}
来源：http://dis.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kux.gzhubu.top

Ruby: def self.f; end
来源：http://ale.tarul.cn

C#:   public static void F() {}
来源：http://gjf.tian-w.cn

[G09] 接口 / 抽象类
来源：http://mwm.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://ndn.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lge.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wfq.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://xsp.yongpay.top

Java: interface Shape { double area(); }
来源：http://myl.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://avu.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://brx.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://nmy.yj20258.top

[G10] 访问控制
来源：http://siz.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://osv.svipenyu.cn

PHP:  public / protected / private
来源：http://qto.meibo888.top

JS:   #private 字段；其余公开
来源：http://jdy.wangshuangyany.cn

TS:   public / protected / private
来源：http://gxe.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://jxo.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gef.aibaodan.cn

Ruby: public / protected / private
来源：http://yxh.gzhubu.top

C#:   public / protected / private / internal
来源：http://jyq.ehwqpu.com

[G11] getter / setter
来源：http://hay.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://far.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://kjk.nanxinkj.top

JS:   get name() { return this._name; }
来源：http://mbi.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://ngs.jyoumei.cn

Java: public String getName() { return name; }
来源：http://iab.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://kgo.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://shl.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://iyh.cheryme.top

[G12] 对象转字符串
来源：http://mze.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://gak.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sqk.yonumen.top

JS:   toString() { return this.name; }
来源：http://gbe.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://njx.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://qjr.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://drj.sxryk.cn

Ruby: def to_s; @name; end
来源：http://ouo.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://wjw.redwolf501.top

[G13] 判断对象类型
来源：http://teq.fzhhl.top

Py:   isinstance(u, User)
来源：http://fjz.pycfn.com

PHP:  $u instanceof User
来源：http://zks.guannengcc.top

JS:   u instanceof User
来源：http://ltu.zhongyouzk.top

TS:   u instanceof User
来源：http://zmf.xylfe.cn

Java: u instanceof User
来源：http://jwl.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://amd.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://fnw.sweek.top

C#:   u is User
来源：http://mbq.mhx1999.top

[G14] 数据类 / record
来源：http://tez.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gtg.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://gaj.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://plb.jinyuanbaomall.cn

TS:   type User = { name: string; age: number };
来源：http://qve.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://lkr.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://aoj.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ksb.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://jft.xuanzx.com

[G15] 枚举
来源：http://trn.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dec.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zyt.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://stu.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fwk.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://fyn.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ujq.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://zng.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dhf.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://zco.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://toc.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://zul.9152youxi.cn

JS:   Object.entries(obj)
来源：http://bry.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://zzd.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eos.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bor.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://mlq.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://wwf.ivvv.top

================================================================================
来源：http://qgi.zhijiandao.cn

H. 异常与错误处理
来源：http://pdn.zhiwuduotai.top

================================================================================
来源：http://xjm.yonumen.top

[H01] try / catch 基础
来源：http://nqd.jinghuilouyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uzp.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sqr.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vqv.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mpm.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rco.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nns.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wlq.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lht.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://fjm.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://svi.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://bez.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://wdp.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eof.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://eyv.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ozh.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://etu.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nar.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://lhp.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://uyo.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jfb.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://hcf.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://fyx.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://gsv.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dzy.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zzi.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://zot.shzxlz.cn

[H04] 自定义异常类型
来源：http://hrz.yj20258.top

Py:   class MyError(Exception): pass
来源：http://idq.iojbl.cn

PHP:  class MyError extends RuntimeException {}
来源：http://drp.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://xus.havefunace.top

TS:   class MyError extends Error {}
来源：http://kxh.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://gay.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://szg.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://vbk.shuidangran.top

C#:   class MyException : Exception {}
来源：http://sls.jinqigfzy.top

[H05] 捕获特定类型
来源：http://nvf.jinqigufen.top

Py:   except ValueError as e:
来源：http://bto.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wnl.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://cyf.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://fbb.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://aid.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vti.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://xqy.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pbb.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://hqo.pengpengdd.cyou

Py:   value = d.get("k") or default
来源：http://sip.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://fpu.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://xwt.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hpj.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hie.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jty.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://zwh.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://tip.zhengqikj.top

[H07] 断言
来源：http://qlo.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://xck.bjfxy.top

PHP:  assert($x > 0);
来源：http://yvt.meibo888.top

JS:   console.assert(x > 0);
来源：http://aax.fktsv.cn

TS:   console.assert(x > 0);
来源：http://sjt.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://cwi.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://key.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://aqv.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://aam.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://vrx.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://spv.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://trd.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://rdu.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vix.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qjf.9152youxi.cn

Go:   err.Error()
来源：http://awp.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://nvl.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://mtk.gaohongyu789.top

[H09] 带错误码的异常
来源：http://evj.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pie.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://usy.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://upu.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tjh.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ypd.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lst.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pli.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xlb.aizwys.cn

[H10] 资源自动释放
来源：http://cvr.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jlx.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rar.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://swk.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iwn.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://znl.bjfxy.top

Go:   defer f.Close()
来源：http://tpk.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tfp.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gre.jianghu66.top

================================================================================
来源：http://gci.c1oappe.top

I. 正则表达式
来源：http://eib.guannengcc.top

================================================================================
来源：http://ljo.0kj1m.cn

[I01] 判断是否匹配
来源：http://nnf.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bms.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iad.wangdashe.top

JS:   /\d+/.test(s)
来源：http://ecu.andypj.xyz

TS:   /\d+/.test(s)
来源：http://bob.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yzu.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rbb.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://hzf.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xts.bjfxy.top

[I02] 提取所有匹配
来源：http://ucw.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://vio.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ydd.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zts.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://zmf.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://chb.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wig.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://kws.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qdf.ppjwa.cn

[I03] 提取捕获分组
来源：http://exs.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ugp.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qkj.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xch.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://glv.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yks.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gno.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vot.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jiv.52xcode.cn

[I04] 正则替换
来源：http://lav.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://drc.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mmk.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mdj.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://cmf.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://enu.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sfh.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://pze.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ivv.yj20258.top

[I05] 按正则拆分
来源：http://jbx.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://duv.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pny.jqgufenzy.top

JS:   s.split(/\s*,\s*/)
来源：http://vru.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://din.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://brp.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rkw.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://xtl.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cxc.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ukd.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zlw.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://viv.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iiq.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://apm.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lcf.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wcn.bbcook.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mlv.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rhp.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://edp.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cme.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yrd.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://plc.shanyushiyangtech.top

TS:   /error/gim
来源：http://kyj.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://coc.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wva.pycfn.com

Ruby: s.scan(/error/i)
来源：http://xui.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fhe.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://vlv.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gri.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://irn.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dhi.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dlo.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pua.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tac.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://buc.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hpo.daria6918.cn

================================================================================
来源：http://you.zdbjq.cn

J. 日期与时间
来源：http://ibf.chenjidiqi.icu

================================================================================
来源：http://bey.yfazqb.com

[J01] 获取当前时间
来源：http://dfh.c1oappe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nha.yongpay.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lzm.xylfe.cn

JS:   new Date();  Date.now()
来源：http://ixs.ybcxt.top

TS:   new Date();  Date.now()
来源：http://fei.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qta.0kj1m.cn

Go:   time.Now()
来源：http://vij.hywenlv.cn

Ruby: Time.now
来源：http://ycs.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rnx.yongpay.top

[J02] 格式化输出
来源：http://oaz.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyj.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uvv.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://thn.ehwqpu.com

TS:   d.toISOString()
来源：http://sav.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zii.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wnx.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yvt.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ewi.yfazqb.com

[J03] 字符串解析为日期
来源：http://jrs.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qmw.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vfr.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://gtj.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://mdw.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://fuf.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mtn.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://wvc.nwbrower.top


<!-- 参考信息 -->
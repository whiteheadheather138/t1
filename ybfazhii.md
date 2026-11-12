代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://plh.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://xuk.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://rue.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://fml.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://giq.smart0.xyz

Ruby: def greet; @name; end
来源：http://qvd.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://qwo.yueranfly.top

[G05] 继承
来源：http://tuh.epnwcf.com

Py:   class Admin(User): pass
来源：http://nlc.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://oek.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://hgj.yueranfly.top

TS:   class Admin extends User {}
来源：http://cmk.316326.xyz

Java: class Admin extends User {}
来源：http://zrv.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pni.daxiang520.top

Ruby: class Admin < User; end
来源：http://dra.yueranfly.top

C#:   class Admin : User {}
来源：http://ffl.bbcook.cn

[G06] 重写方法
来源：http://fqg.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://jlp.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zgp.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://hlk.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://vff.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://prp.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lsp.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://dqw.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://uot.tarul.cn

[G07] 调用父类方法
来源：http://xcz.zhengqikj.top

Py:   super().greet()
来源：http://cvl.yvedp.cn

PHP:  parent::greet();
来源：http://glw.sweek.top

JS:   super.greet();
来源：http://zhi.hfpthk.cn

TS:   super.greet();
来源：http://uyb.fktsv.cn

Java: super.greet();
来源：http://sgx.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mir.hysaishi.cn

Ruby: super
来源：http://bgi.daxiang520.top

C#:   base.Greet();
来源：http://yzw.xylfe.cn

[G08] 静态方法与属性
来源：http://ezs.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mbx.ivvv.top

PHP:  public static function f() {}
来源：http://cai.birdmap.top

JS:   static f() {}
来源：http://yws.sufxvd.cn

TS:   static f(): void {}
来源：http://pae.fengsongda.top

Java: static void f() {}
来源：http://yzb.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zqf.chenjidiqi.icu

Ruby: def self.f; end
来源：http://apf.yj202588.top

C#:   public static void F() {}
来源：http://ybl.hammf.cn

[G09] 接口 / 抽象类
来源：http://rba.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://lsj.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://frq.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kau.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://umm.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://ixz.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://etw.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ubl.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://nka.chenlongwang.top

[G10] 访问控制
来源：http://aqx.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://hnq.sjlbkw.cn

PHP:  public / protected / private
来源：http://xfp.fehbvm.com

JS:   #private 字段；其余公开
来源：http://ely.jlsjyb.cn

TS:   public / protected / private
来源：http://gkf.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://nnq.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://trl.quarkkingdee.top

Ruby: public / protected / private
来源：http://pgl.sxryk.cn

C#:   public / protected / private / internal
来源：http://gqb.jinyuanbaomall.cn

[G11] getter / setter
来源：http://bog.daria6918.cn

Py:   @property 与 @x.setter
来源：http://duo.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oib.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://vex.sweek.top

TS:   get name(): string { return this._name; }
来源：http://egm.52xcode.cn

Java: public String getName() { return name; }
来源：http://kjv.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hzd.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://lvy.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://oii.hesvh.cn

[G12] 对象转字符串
来源：http://ayb.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://esm.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nck.smart0.xyz

JS:   toString() { return this.name; }
来源：http://zjo.hywenlv.cn

TS:   toString(): string { return this.name; }
来源：http://wci.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://teq.meibo888.top

Go:   func (u User) String() string { return u.Name }
来源：http://jxs.yvedp.cn

Ruby: def to_s; @name; end
来源：http://lbm.yj20258.top

C#:   public override string ToString() => Name;
来源：http://sew.gaohongyu789.top

[G13] 判断对象类型
来源：http://kmm.dashuyun.cn

Py:   isinstance(u, User)
来源：http://ufa.guannengcc.top

PHP:  $u instanceof User
来源：http://omg.tian-w.cn

JS:   u instanceof User
来源：http://nab.yuxming.cn

TS:   u instanceof User
来源：http://dml.zhengqikj.top

Java: u instanceof User
来源：http://ifd.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jwa.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://hlo.yanxiufei.cn

C#:   u is User
来源：http://isl.cucudq.cn

[G14] 数据类 / record
来源：http://hxy.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://omt.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://zna.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://iqa.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://kkr.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://ljc.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://jkn.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://trw.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://wji.svipenyu.cn

[G15] 枚举
来源：http://mpw.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ujp.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xsw.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ynw.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ogq.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://dyz.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ywt.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://xcs.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yse.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://ipg.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dyl.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://nub.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://nyu.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://adz.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pbm.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dco.cheryme.top

Ruby: obj.instance_variables
来源：http://lek.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://lcp.yongpay.top

================================================================================
来源：http://lcl.jlsjyb.cn

H. 异常与错误处理
来源：http://tyb.yj20258.top

================================================================================
来源：http://mri.hammf.cn

[H01] try / catch 基础
来源：http://qmk.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eoi.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gtg.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://glo.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dtx.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jgu.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://egz.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ntm.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xtw.vehdjk.com

[H02] finally / ensure 收尾
来源：http://bwu.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://foc.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://efz.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jtg.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://htb.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eua.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bar.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mhb.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uqg.iojbl.cn

[H03] 主动抛出异常
来源：http://arz.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://ckw.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://slk.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://sgj.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://txo.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hpp.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zmn.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gyt.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qtt.yanxiufei.cn

[H04] 自定义异常类型
来源：http://efa.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://jpe.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kqq.gzhubu.top

JS:   class MyError extends Error {}
来源：http://zep.wangshuangyany.cn

TS:   class MyError extends Error {}
来源：http://bra.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://bjb.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xir.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://hfi.tian-w.cn

C#:   class MyException : Exception {}
来源：http://jmi.uphjek.com

[H05] 捕获特定类型
来源：http://mbf.havefunace.top

Py:   except ValueError as e:
来源：http://jhk.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lbc.xinyue.icu

JS:   if (e instanceof TypeError) {}
来源：http://cdd.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://waw.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://bgn.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mqe.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://rmr.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jrv.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://bzk.svipenyu.cn

Py:   value = d.get("k") or default
来源：http://tch.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://wpt.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://knx.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dho.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lzf.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hws.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://wep.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://ikg.hnqzz.top

[H07] 断言
来源：http://jjh.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://gdz.svipenyu.cn

PHP:  assert($x > 0);
来源：http://itq.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://ocl.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://rid.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://ttw.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wdn.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lxo.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://vrm.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://aeq.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://nan.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jxy.shuidangran.top

JS:   e.message;  e.stack
来源：http://zor.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pha.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rgl.hongshengwenyu.top

Go:   err.Error()
来源：http://wcc.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://ppi.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://asg.ybcxt.top

[H09] 带错误码的异常
来源：http://eqt.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ovg.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://brz.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mmg.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://azm.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ihy.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zvz.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://hjr.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://opi.nanxuanxn.top

[H10] 资源自动释放
来源：http://cyo.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nlj.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://phi.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nnb.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qrp.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hfk.zdqjudy.top

Go:   defer f.Close()
来源：http://wsj.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mwg.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ade.hysaishi.cn

================================================================================
来源：http://ieg.cqqwz.cn

I. 正则表达式
来源：http://jdy.haohaochexian.top

================================================================================
来源：http://fpm.yangfankeji.com

[I01] 判断是否匹配
来源：http://efn.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yns.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://vpv.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://kqh.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://ibb.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hid.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gpx.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://vzm.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pkk.tanke756.top

[I02] 提取所有匹配
来源：http://psy.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://hyk.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wuc.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nvv.iojbl.cn

TS:   s.match(/\d+/g)
来源：http://fmd.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uxl.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aug.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://ehs.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sph.cqqwz.cn

[I03] 提取捕获分组
来源：http://qxz.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mqb.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tsu.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pgb.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sdd.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://emr.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ugs.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rbm.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cwu.jqgfzy.top

[I04] 正则替换
来源：http://abt.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ztn.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vuj.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kfd.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://dyp.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zba.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hjw.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://txc.xuanzx.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kzj.pengpengdd.cyou

[I05] 按正则拆分
来源：http://iuc.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mfh.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nxu.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://bkd.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://dkx.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://xss.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xho.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ovb.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fit.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rqp.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mln.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bzg.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wfc.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hjd.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pyl.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tnx.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://epx.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vfi.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://zmk.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iae.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cnt.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jkx.jinqigufen.top

TS:   /error/gim
来源：http://ygj.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dag.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zxy.fehbvm.com

Ruby: s.scan(/error/i)
来源：http://qap.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fsk.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://uqj.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kpx.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fda.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://axq.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tik.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ajn.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dyv.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://imf.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ocn.zhaomingkeji.xyz

================================================================================
来源：http://yzt.yuanzhike.top

J. 日期与时间
来源：http://qhc.yuxming.cn

================================================================================
来源：http://vum.yj20258.top

[J01] 获取当前时间
来源：http://hnf.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mvx.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eqr.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://bak.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://tqd.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jyk.uphjek.com

Go:   time.Now()
来源：http://yag.316326.xyz

Ruby: Time.now
来源：http://tfs.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://raa.cqqwz.cn

[J02] 格式化输出
来源：http://vwj.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://euj.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tfl.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gtf.hnqzz.top

TS:   d.toISOString()
来源：http://qyd.tanke756.top


<!-- 参考信息 -->